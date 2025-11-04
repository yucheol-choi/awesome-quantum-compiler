## Awesome Quantum Compiler
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://GitHub.com/Naereen/ama)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yucheol-choi/)

### Description
For those who are either new to or currently researching in the field of quantum compilers, I will be regularly updating resources such as papers categorised by subtopics, open-source code, learning materials(currently planning to create it myself) on quantum compilers, as well as my own personal research paper reviews. I'm still a first-year PhD student, so I have many shortcomings. Feel free to provide any feedback on mistakes.


## Table of Contents
- [Survey papers](#survey-papers)
- [Part A: Compilation Flow — From Algorithm to Pulse](#part-a-compilation-flow--from-algorithm-to-pulse)
  - [Language & Logical IR](#language-logical-ir)
  - [Hardware-Agnostic Optimization](#hardware-agnostic-optimization)
  - [Hardware-Aware Compilation & Mapping](#hardware-aware-compilation--mapping)
  - [Pulse-Level Compilation & Control](#pulse-level-compilation--control)
  - [Runtime & Dynamic Execution](#runtime--dynamic-execution)
- [Part B: Quantum Compiler Ecosystem](#part-b-quantum-compiler-ecosystem)
  - [Quantum Testing and Debugging](#quantum-testing-and-debugging)
  - [Quantum Formal Verification](#quantum-formal-verification)
  - [QEC-aware Compilation](#qec-aware-compilation)
  - [Quantum Secure Compilation](#quantum-secure-compilation)
  - [Quantum Circuit Analysis](#quantum-circuit-analysis)
- [Part C: Quantum Compiler Niche Fields](#part-c-quantum-compiler-niche-fields)
  - [Topological Quantum Compilation](#topological-quantum-compilation)
  - [Qudit Compilation](#qudit-compilation)
  - [Quantum Circuit Obfuscation](#quantum-circuit-obfuscation)
  - [Measurement-Based Quantum Compilation](#measurement-based-quantum-compilation)
- [Part D: Conference and Journal](#part-d-conference-and-journal) 
  - [Top-tier Conference Deadline](#conference-deadline)
  - [Journals](#journals)
</br>
 
<h2 id="survey-papers">Survey papers</h2>

+ [Quantum Compilation Process: A Survey](https://link.springer.com/chapter/10.1007/978-3-031-90200-0_9) - F. Javier Cardama, Jorge Vázquez-Pérez, Tomás F. Pena, Juan C. Pichel & Andrés Gómez, 2025
+ [Quantum Compiler Design for Qubit Mapping and Routing](https://arxiv.org/pdf/2505.16891) - Chenghong zhu et al., 2025.
+ [A Comprehensive Review of Quantum Circuit Optimization: Current Trends and Future Directions](https://www.mdpi.com/2624-960X/7/1/2) - Krishnageetha Karuppasamy et al., 2025.
+ [Quantum Circuit Synthesis and Compilation Optimization: Overview and Prospects](https://arxiv.org/html/2407.00736v1) - Ge Yan et al., 2024.
+ [Quantum Compiling](https://arxiv.org/abs/2112.00187) - Marco Maronese, Lorenzo Moro, Lorenzo Rocutto, Enrico Prati, 2021
+ [Programming languages and compiler design for realistic quantum hardware](https://www.nature.com/articles/nature23459) - Frederic T. Chong, Diana Franklin, Margaret Martonosi, Nature, 2017
</br>


## Part A: Compilation Flow — From Algorithm to Pulse

<h4 id="language-logical-ir">Language & Logical IR</h4>

> IR Design & Transpilation Frameworks 
+ [PHOENIX: Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) - Zhaohui Yang et al., 2025  - [GitHub](https://github.com/iqubit-org/phoenix)  
+ [LinguaQuanta: Towards a Quantum Transpiler Between OpenQASM and Quipper](https://arxiv.org/pdf/2404.08147) - Scott Wesley et al., 2024  - [GitHub](https://github.com/onestruggler/qasm-quipper) 
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) - Anurudh Peduri, Siddharth Bhat, CC 2022  - [GitHub](https://github.com/opencompl/QMLIR)  
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) - David Ittah et al., 2021  - [GitHub](https://github.com/dime10/QIRO)  
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) - Alexander McCaskey, Thien Nguyen, QCE 2021
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) - Ali JavadiAbhari et al., 2014  - [GitHub](https://github.com/epiqc/ScaffCC)  


> Loop & Control-Flow Transforms 
+ [The Limits of Control Flow in Quantum Programming](https://arxiv.org/abs/2304.15000) – Charles Yuan et al., OOPSLA, 2023
+ [Software Pipelining for Quantum Loop Programs](https://arxiv.org/abs/2012.12700) – Jingzhe Guo, Mingsheng Ying, IEEE TSE, 2023
+ [Exploring the Impact of Affine Loop Transformations in Qubit Allocation](https://arxiv.org/pdf/2010.11999) – Martin Kong, QCS, 2020
  


<h4 id="hardware-agnostic-optimization">Hardware-Agnostic Optimization</h4>

> Quantum Program Optimization 
+ [SuperstaQ: Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) - Campbell et al., QCE 2023 - [GitHub](https://github.com/Infleqtion/client-superstaq)  
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/2109.03371) - Gushu Li et al., 2021
+ [Enabling Dataflow Optimization for Quantum Programs](https://arxiv.org/abs/2101.11030) - David Ittah et al., 2021
+ [A Meet-in-the-Middle Algorithm for Fast Synthesis of Depth-Optimal Quantum Circuits](https://arxiv.org/abs/1206.0758) - Matthew Amy et al., 2021
+ [Automated optimization of large quantum circuits with continuous parameters](https://arxiv.org/abs/1710.07345) - Yunseong Nam et al., 2017  - [GitHub](https://github.com/njross/optimizer)  
+ [A software methodology for compiling quantum programs](https://arxiv.org/abs/1604.01401) - Thomas Häner et al., 2016
+ [Exact synthesis of single-qubit unitaries over Clifford-cyclotomic gate sets](https://arxiv.org/abs/1501.04944) - Simon Forest et al., 2015
+ [Polynomial-Time T-Depth Optimization of Clifford+T Circuits Via Matroid Partitioning](https://arxiv.org/abs/1303.2042) - Matthew Amy et al., 2013
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/abs/1810.00375) - Häner, Hoefler, Troyer, OOPSLA 2013
+ [Repeat-until-Success: Non-Deterministic Decomposition of Single-Qubit Unitaries](https://arxiv.org/abs/1311.1074) - Adam Paetznick, Krysta Svore, 2013  - [GitHub (sample)](https://github.com/microsoft/Quantum/tree/main/samples/algorithms/repeat-until-success)  
+ [Circuit for Shor’s Algorithm Using 2n+3 Qubits](https://arxiv.org/abs/quant-ph/0205095) - Stephane Beauregard, 2002


> Circuit Optimisation 
+ [A Resource-Allocating Compiler for Lattice Surgery](https://arxiv.org/abs/2506.04620) - Alan Robertson, Haowen Gao, Yuval R. Sanders, 2025.  - [GitHub](https://github.com/latticesurgery-com/lattice-surgery-compiler)  
+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) - Francisco J. R. Ruiz, Nature Machine Intelligence, 2025. - [GitHub](https://github.com/google-deepmind/alphatensor_quantum)  
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) - Zikun Li et al., OOPSLA, 2024.  - [GitHub](https://github.com/quantum-compiler/Quarl) 
+ [Machine Learning Optimization of Quantum Circuit Layouts](https://dl.acm.org/doi/full/10.1145/3565271) - Alexandru Pale et al., ACM TQC, 2023.  - [GitHub](https://github.com/alexandrupaler/qxx)  
+ [Synthesizing Quantum-Circuit Optimizers](https://dl.acm.org/doi/abs/10.1145/3591254) - Amanda Xu et al., PLDI, 2023.  - [GitHub](https://github.com/qqq-wisc/queso)
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) - Bodo Rosenhahn, Tobias J. Osborne, 2023



<h4 id="hardware-aware-compilation-mapping">Hardware-Aware Compilation & Mapping</h4>

Hardware Platforms
> Superconducting QC
+ [Selective Excitation of Superconducting Qubits with a Shared Control Line through Pulse Shaping](https://arxiv.org/pdf/2501.10710) - Ryo Matsuda et al., 2025
+ [Virtual-Z Gates and Symmetric Gate Compilation](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.020348) - Arian Vezvaee et al., 2025
+ [Qibosoq: RFSoC Control Software for Self-Hosted Quantum Hardware via QICK](https://arxiv.org/abs/2310.05851) - Andrea Pasquale et al., 2025 - [GitHub](https://github.com/qiboteam/qibosoq)
+ [CCMap: Hardware-Aware Compilation for Chip-to-Chip Coupler-Connected QPUs](https://arxiv.org/abs/2505.09036) - Zefan Du et al., Arxiv, 2025
+ [Pulse-Based Variational Quantum Optimization and Metalearning in Superconducting Circuits](https://arxiv.org/abs/2407.12636) - Yapeng Wang et al., 2024
+ [Direct Pulse-Level Compilation of Arbitrary Quantum Logic Gates on Superconducting Qutrits](https://arxiv.org/abs/2303.04261) - Yujin Cho et al., , Physical Review Applied, 2024
+ [Sensitivity-Adapted Closed-Loop Optimization for High-Fidelity CZ Gates](https://arxiv.org/abs/2412.17454) - Niklas J. Glaser et al., 2024
+ [Implementing Fast and High-Fidelity Quantum Operations Using Open-Loop Optimal Control](https://arxiv.org/abs/2410.22603) - LBNL Collaboration, 2024
+ [Qibolab: An Open-Source Hybrid Quantum Operating System](https://quantum-journal.org/papers/q-2024-02-12-1247/) - Stavros Efthymiou et al., Quantum Journal 2024, [GitHub](https://github.com/qiboteam/qibolab)
+ [Qibocal: An Open-Source Framework for Calibration of Self-Hosted Quantum Devices](https://arxiv.org/abs/2410.00101) - Andrea Pasquale et al., 2024  - [GitHub](https://github.com/qiboteam/qibocal)
+ [A Time Optimization Framework for Robust and Low-Latency Quantum Circuits](https://arxiv.org/abs/2412.18533) - Eduardo W. Lussi et al., Physical Review Applied, 2024
 
> Ion-Trap QC
+ [Graph-Based Pulse Representation for Diverse Quantum Control Hardware](https://arxiv.org/abs/2409.08407) - Aniket S. Dalvi et al., 2024
+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) - Francesco Preti,. Quantum Journal, 2024
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) - Jonathan Durandau, Quantum, 2023. [GitHub](https://github.com/cda-tum/mqt-ion-shuttler)  [oai_citation:2‡GitHub](https://github.com/cda-tum/mqt-ion-shuttler)
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) - Fabian Kreppel et al., 2022
+ [Backend compiler phases for trapped-ion quantum computers](https://arxiv.org/abs/2206.00544) - T. Schmale et al., 2022
  
> Neutral-Atom QC
+ [Pulse Family Optimization for Parametrized Quantum Gates Using Spectral Clustering](https://arxiv.org/abs/2408.00119) - Robert de Keijzer et al., Quantum Journal, 2024
+ [Q-Pilot: Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) - Hanrui Wang., DAC, 2024.
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) - S. Ebadi et al., Science(Journal), 2022.  - [GitHub]

> Photonics QC
+ [OneAdapt: Adaptive Compilation for Resource-Constrained Photonic One-Way Quantum Computing](https://arxiv.org/abs/2504.17116) - Hezi Zhang et al., 2025
+ [A Scalable and Robust Compilation Framework for Emitter-Photonic Quantum Computing](https://arxiv.org/abs/2503.16346) - Xiangyu Ren et al., 2025
+ [OnePerc: A Randomness-aware Compiler for Photonic Quantum Computing](https://arxiv.org/abs/2403.01829) - Hezi Zhang et al., 2024
+ [OneQ: A Compilation Framework for Photonic One-Way Quantum Computation](https://arxiv.org/abs/2209.01545) - Hezi Zhang et al., ISCA, 2023
+ [A Compiler for Universal Photonic Quantum Computers](https://arxiv.org/abs/2210.09251) - Felix Zilk et al., QCS, 2022

Compilation Techniques
> Circuit Scheduling 
+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) - Toshinari Itoko, Takashi Imamichi, QCE, 2020
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) - Gian Giacomo Guerreschi, Jongsoo Park, Quantum Sci, 2017

> Qubit Mapping & Routing 
+ [S-SYNC: Shuttle & SWAP Co-Optimisation in QCCD](https://arxiv.org/abs/2505.01316) - Chenghong Zhu, Xian Wu, Jingbo Wang, Xin Wang, ISCA 2025
+ [Compiling quantum circuits for dynamically field-programmable neutral atoms array processors](https://arxiv.org/pdf/2306.03487.pdf) - D. B. Tan et al., 2024
+ [Qubit mapping for reconfigurable atom arrays](https://dl.acm.org/doi/abs/10.1145/3508352.3549331) - B. Tan et al, ICCAD, 2022
+ [Qubit Mapping and Routing via MaxSAT](https://arxiv.org/abs/2208.13679v1) - Abtin Molavi, Amanda Xu, Martin Diges, Lauren Pick, Swamit Tannu, Aws Albarghouthi, MICRO, 2022
+ [QuCloud: A New Qubit Mapping Mechanism for Multi-programming Quantum Computing in Cloud Environment](https://ieeexplore.ieee.org/document/9407180) - Lei Liu, Xinglei Dou, HPCA, 2021
+ [Optimal mapping for near-term quantum architectures based on Rydberg atoms](https://arxiv.org/abs/2109.04179) - S.Brandhofer et al., ICCAD, 2021
+ [Time-optimal Qubit mapping](https://dl.acm.org/doi/pdf/10.1145/3445814.3446706) - Chi Zhang et al., ASPLOS, 2021
+ [Not All Qubits Are Created Equal: A Case for Variability-Aware Policies for NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007) - Swamit S. Tannu, Moinuddin K. Qureshi, ASPLOS, 2019
+ [Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.](https://arxiv.org/abs/1901.11054) - Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi, ASPLOS, 2019


<h4 id="pulse-level-compilation-control">Pulse-Level Compilation & Control</h4>

+ [A Synergistic Compilation Workflow for Tackling Crosstalk in Quantum Machines](https://arxiv.org/abs/2207.05751) - Fei Hua et al., 2023
+ [Hybrid Gate-Pulse Model for Variational Quantum Algorithms](https://arxiv.org/abs/2212.00661) - Zhiding Liang et al. 2022
+ [Resource-Efficient Quantum Computing by Breaking Abstractions](https://arxiv.org/abs/2011.00028) - Yunong Shi, IEEE Journal, 2020.  
+ [Optimized Quantum Compilation for Near-Term Algorithms with OpenPulse](https://arxiv.org/abs/2004.11205) Pranav Gokhale et al, 2020.

<h4 id="runtime-dynamic-execution">Runtime & Dynamic Execution</h4>

+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) - Philipp Seitz et al., QCE, 2024 - [GitHub](https://github.com/qc-tum/milq) 
+ [Qibolab: An Open-Source Hybrid Quantum Operating System](https://quantum-journal.org/papers/q-2024-02-12-1247/) - Stavros Efthymiou et al., Quantum Journal, 2024  - [GitHub](https://github.com/qiboteam/qibolab)  
+ [Combining Quantum Processors with Real-Time Classical Communication](https://www.nature.com/articles/s41586-024-08178-2) - Almudena Carrera Vazquez et al., Nature, 2024. - [GitHub](https://github.com/eggerdj/cut_graph_state_data) 

<h2 id="part-b-quantum-compiler-ecosystem">Part B: Quantum Compiler Ecosystem</h2>

<h4 id="quantum-testing-and-debugging">Quantum Testing and Debugging</h4>

+ [Testing and Debugging Quantum Programs: The Road to 2030](https://dl.acm.org/doi/10.1145/3715106) — Neilson Carlos Leite Ramalho et al, TOSEM, 2025.
+ [QuraTest: Automated Testing of Quantum Programs with Complex Input States](https://dl.acm.org/doi/10.1109/ASE56229.2023.00196) — Jiaming Ye et al. ASE 23.
+ [MorphQ: Metamorphic Testing for Quantum Programs](https://arxiv.org/abs/2206.01111) — Matteo Paltenghi, Michael Pradel ICSE 23. 
+ [QuCAT: Quantum Combinatorial Testing Framework](https://arxiv.org/abs/2309.00119) — Xinying Wang et al. ASE 23.
+ [QuSBT: Search-Based Testing of Quantum Programs](https://dl.acm.org/doi/10.1145/3510454.3516839) — Xinying Wang et al, ICSE 22.
+ [QMutPy: A Mutation Testing Tool for Quantum Algorithms and Applications in Qiskit](https://jose.github.io/assets/pdfs/ISSTA2022-tool-paper.pdf) — E. Fortunato, et al. ASE 22.
+ [Quito: a coverage-guided test generator for quantum programs](https://dl.acm.org/doi/abs/10.1109/ASE51524.2021.9678798) — Xinyi Wang et al. (2021). ASE 21.
+ [Muskit: Mutation Testing for Qiskit Quantum Programs](https://ieeexplore.ieee.org/document/9678563) — A. Mendiluze, et al. ASE 21 
+ [Statistical Assertions for Quantum Programs](https://arxiv.org/abs/1905.09721) — H.-L. Huang, M. Martonosi, ISCA 19.
+ [Projection-based runtime assertions for testing and debugging Quantum programs](https://dl.acm.org/doi/10.1145/3428218) — Gushu Li et al. OOPSLA 2020.
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/pdf/1810.00375) — Thomas Häner et al, OOPSLA, 2020

<h4 id="quantum-formal-verification">Quantum Formal Verification</h4>

+ [CoqQ: Foundational Verification of Quantum Programs](https://arxiv.org/abs/2207.11350) — L. Zhou, G. Barthe, P.-Y. Strub, J. Liu, M. Ying (2022). 
+ [Twist: Sound Reasoning for Purity and Entanglement in Quantum Programs](https://arxiv.org/abs/2205.02287) — C. Yuan, C. McNally, M. Carbin (2022). Proceedings of the ACM on Programming Languages (POPL)
+ [An Algebraic Method to Fidelity-based Model Checking over Quantum Markov Chains](https://arxiv.org/abs/2101.04971) — M. Xu, J. Fu, J. Mei, Y. Deng (2021). 
+ [Quantum Relational Hoare Logic](https://arxiv.org/abs/1802.03188) — D. Unruh (2019). Proceedings of the ACM on Programming Languages (POPL)
+ [ProbReach: Verified Probabilistic Delta-Reachability for Stochastic Hybrid Systems](https://arxiv.org/abs/1410.8060) — F. Shmarov, P. Zuliani (2015). (HSCC)
+ [Formal Verification of Quantum Algorithms Using Quantum Hoare Logic](https://link.springer.com/chapter/10.1007/978-3-030-25543-5_12) — J. Liu, B. Zhan, S. Wang, S. Ying, T. Liu, Y. Li, M. Ying, N. Zhan (2019). Computer Aided Verification (CAV)
+ [Quantum relational Hoare logic](https://dl.acm.org/doi/10.1145/3290346) — J. Liu, B. Zhan, S. Wang, S. Ying, T. Liu, Y. Li, M. Ying, N. Zhan (2019). (POPL)
+ [QWIRE: A Core Language for Quantum Circuits](https://dl.acm.org/doi/10.1145/3009837.3009894) — J. Paykin, R. Rand, S. Zdancewic (2017). Proceedings of the ACM on Programming Languages (POPL)
+ [Floyd-Hoare Logic for Quantum Programs](https://dl.acm.org/doi/10.1145/2049706.2049708) — M. Ying (2011). ACM Transactions on Programming Languages and Systems (TOPLAS)
+ [An Algebra of Quantum Processes](https://arxiv.org/abs/0707.0330) — M. Ying, Y. Feng, R. Duan, Z. Ji (2009) (TOCL)
+ [A Logic for Formal Verification of Quantum Programs](https://dl.acm.org/doi/10.1007/978-3-642-10622-4_7) — M. Ying, Y. Feng, R. Duan, Z. Ji (2009). Advances in Computer Science – ASIAN 2009 (Springer)
+ [Towards a Quantum Programming Language](https://dl.acm.org/doi/10.1017/S0960129504004256) — P. Selinger (2004). Mathematical Structures in Computer Science

<h4 id="qec-aware compilation">QEC-Aware Compilation</h4>

+ [Resource-Efficient Context-Aware Dynamical Decoupling Embedding for Arbitrary Large-Scale Quantum Algorithms](https://link.aps.org/doi/10.1103/PRXQuantum.6.010332), Paul Coote et al., PRX Quantum, 2025
+ [Learning high-accuracy error decoding for quantum processors](https://www.nature.com/articles/s41586-024-08148-8) - Johannes Bausch et al., Nature, 2024
+ [Error Propagation-Aware Routing: A New Routing Strategy to Improve Success Rates of Quantum Circuits](https://dl.acm.org/doi/pdf/10.1145/3649476.3658790), Lu Fang et al., ICCAD, 2024 
+ [Learning How to Dynamically Decouple](https://arxiv.org/html/2405.08689v1), Arefur Rahman et al., arXiv, 2024.
+ [On the Use of Calibration Data in Error-Aware Compilation Techniques for NISQ Devices](https://arxiv.org/html/2407.21462v1), Handy Kurniawan et al., arXiv, 2024.
+ [TISCC: A Surface Code Compiler and Resource Estimator for Trapped-Ion Processors](https://dl.acm.org/doi/abs/10.1145/3624062.3624214) - Tyler Leblond, Ryan S. Bennink, Justin G. Lietz, and Christopher M. Seck, SC, 2023
+ [Qubit Mapping and Routing via MaxSAT](https://pages.cs.wisc.edu/~amolavi/files/micro22.pdf), Maryam Amiri et al., MICRO, 2022.
+ [VAQEM: A Variational Approach to Quantum Error Mitigation](https://www.computer.org/csdl/proceedings-article/hpca/2022/202700a288/1Ds0fvoYbCw) - Gokul S. Ravi et al., HPCA, 2022
+ [Exploiting Long-Distance Interactions and Tolerating Atom Loss in Neutral Atom Quantum Architectures](https://arxiv.org/pdf/2111.06469.pdf) - Jonathan M. Baker, et al., ISCA, 2021
+ [ADAPT: Mitigating Idling Errors in Qubits via Adaptive Dynamical Decoupling](https://dl.acm.org/doi/10.1145/3466752.3480059) - Poulami Das et al., MICRO, 2021
+ [A Noise-Aware Qubit Mapping Algorithm Evaluated via Qubit Interaction-Graph Criteria](https://www.researchgate.net/publication/350512755_A_Noise-Aware_Qubit_Mapping_Algorithm_Evaluated_via_Qubit_Interaction-Graph_Criteria) - Matthew Steinberg et al., arXiv, 2021.
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) - Xin-Chuan Wu, Dripto M Debroy, Yongshan Ding, Jonathan M Baker, Yuri Alexeev, Kenneth R Brown, and Frederic T Chong, HPCA, 2020
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503), Yongshan Ding, Pranav Gokhale, Sophia Fuhui Lin, Richard Rines, Thomas Propson, Frederic T. Chong, MICRO, 2020
+ [Digital Zero-Noise Extrapolation for Quantum Error Mitigation](https://arxiv.org/abs/2005.10921), Tudor Giurgica-Tiron et al., IEEE QCE, 2020 
+ [Near-Optimal Routing of Noisy Quantum States](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/11134/111340A/Near-optimal-routing-of-noisy-quantum-states/10.1117/12.2526670.short), Kyle Cote et al., SPIE Proc., 2019.
+ [Not All Qubits Are Created Equal: Variation-Aware Qubit Allocation in NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007), Swamit Tannu & Moinuddin Qureshi, ASPLOS, 2019
+ [Practical Quantum Error Mitigation for Near-Future Applications](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509), Suguru Endo et al., Phys. Rev. X, 2018.  
+ [Error Mitigation for Short-Depth Quantum Circuits](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509), Kristan Temme et al., Phys. Rev. Lett., 2017.




<h4 id="quantum-secure-compilation">Quantum Secure Compilation</h4>

+ [Split Compilation for Security of Quantum Circuits](https://pure.psu.edu/en/publications/split-compilation-for-security-of-quantum-circuits) — Abdullah Ash Saki, Aakarshitha Suresh, Rasit Onur Topaloglu, Swaroop Ghosh. ICCAD 2021.  ￼
+ [A Quantum Circuit Obfuscation Methodology for Security and Privacy](https://arxiv.org/abs/2104.05943) — Aakarshitha Suresh, Abdullah Ash Saki, Mahabubul Alam, Rasit Onur Topaloglu, Swaroop Ghosh. HASP @ MICRO 2021.  ￼
+ [OpaQue: Program Output Obfuscation for Quantum Software Circuits in Quantum Clouds](https://hpcrl.github.io/ICS2025-webpage/program/Proceedings_ICS25/ics25-32.pdf) — Tirthak Patel, Aditya Ranjan, Daniel Silver, Harshitta Gandhi, William Cutler, Devesh Tiwari. ICS 2025.  ￼
+ [TetrisLock: Quantum Circuit Split Compilation with Interlocking Patterns](https://arxiv.org/abs/2503.11982) — Qian Wang, Jayden John, Ben Dong, Yuntao Liu. arXiv 2025 (preprint).  ￼
+ [OPAQUE: Obfuscating Phase in Quantum Circuit Compilation for Efficient IP Protection](https://www.arxiv.org/abs/2502.16605) — Anees Rehman, Vincent Langford, Yuntao Liu. ISQED 2025.  ￼
+ [Encrypted-state quantum compilation scheme based on quantum circuit obfuscation](https://arxiv.org/abs/2507.17589) — Chenyi Zhang, Tao Shang, Xueyi Guo, Yuanjing Zhang. arXiv 2025.  ￼￼
+ [Quantum Homomorphic Encryption for Circuits of Low T-gate Complexity](https://link.springer.com/chapter/10.1007/978-3-662-48000-7_30) — Anne Broadbent, Stacey Jeffery. CRYPTO 2015.  ￼
+ [Unconditionally Verifiable Blind Quantum Computation](https://journals.aps.org/pra/pdf/10.1103/PhysRevA.96.012303) — Joseph F. Fitzsimons, Elham Kashefi. Physical Review A, 2017. 


<h4 id="quantum-circuit-analysis">Quantum Circuit Analysis</h4>

+ [Character Complexity: A Novel Measure for Quantum Circuit Analysis](https://arxiv.org/abs/2408.09641) - Daksh Shami, 2024
+ [QuCT: A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) - Siwei Tan et al., MICRO 2023  - [GitHub](https://github.com/JanusQ/QuCT-Micro2023) 
+ [Quantum Vulnerability Analysis to Guide Robust Quantum Computing System Design](https://arxiv.org/pdf/2207.14446) - Fang Qi et al., 2023


<h2 id="part-c-quantum-compiler-niche-fields">Part C: Quantum Compiler Niche Fields</h2>

<h4 id="topological-quantum-compilation">Topological Quantum Compilation</h4>

+ [Topological quantum compilation of two-qubit gates](https://arxiv.org/abs/2408.07132) — Parsa Hosseini et al. (2024). 
+ [Topological quantum compilation of metaplectic anyons based on the genetic optimized algorithms](https://arxiv.org/abs/2501.01745) — Parsa Hosseini et al. (2025). 
+ [Optimized Topological Quantum Compilation of Three-Qubit Controlled Gates in the Fibonacci Anyon Model](https://arxiv.org/abs/2311.17645) — Parsa Hosseini et al. (2023).
+ [Topological Quantum Gates in Homotopy Type Theory](https://arxiv.org/abs/2303.02382) — Guillaume Munch-Madewig et al. (2023). 
+ [Systematic Computation of Braid Generator Matrix in Topological Quantum Computation](https://arxiv.org/abs/2307.01892) — Parsa Hosseini et al. (2023). 
+ [Asymptotically Optimal Topological Quantum Compiling](https://arxiv.org/abs/1310.4150) — Michael Freedman et al., Mathematical Physics Journal (2013). 
+ [Provably Optimal Quantum Circuits with Mixed-Integer Programming](https://arxiv.org/abs/2510.00649) — Yufei Ding et al. (2025). 

<h4 id="qudit-compilation">Qudit Compilation</h4>

+ [Efficient, direct compilation of SU(N) operations into SNAP](https://arxiv.org/abs/2307.11900) — Vladislav D. Kurpas et al., Physical Review A, (2023). 
+ [QudCom: Towards Quantum Compilation for Qudit Systems](https://arxiv.org/abs/2311.07015) — Sebastian Brandhofer et al. (2023). 
+ [Adaptive Compilation of Multi-Level Quantum Operations](https://arxiv.org/abs/2206.03842) — David R. M. Arvidsson-Shukur et al. (2022). 
+ [Compilation of Entangling Gates for High-Dimensional Quantum Processors](https://arxiv.org/abs/2301.04155) — Manuel G. J. B. A. Cordier et al. (2023). 
+ [MQT Qudits: A Software Framework for Mixed-Dimensional Quantum Computing](https://arxiv.org/abs/2410.02854) — Lukas Burgholzer et al. (2024). 

<h4 id="quantum-circuit-obfuscation">Quantum Circuit Obfuscation</h4>

+ [Quantum state obfuscation from classical oracles](https://dl.acm.org/doi/abs/10.1145/3618260.3649673) - J. Bartusek, Z. Brakerski, V. Vaikuntanathan, CCS, 2024
+ [Obfuscation of pseudo-deterministic quantum circuits](https://dl.acm.org/doi/abs/10.1145/3564246.3585179) - J. Bartusek, F. Kitagawa, R. Nishimaki, ACM Symposium on Theory of Computing (STOC), 2023  
+ [Indistinguishability obfuscation of null quantum circuits and applications](https://arxiv.org/abs/2106.06094) - J. Bartusek, G. Malavolta, ITCS, 2021
+ [A quantum circuit obfuscation methodology for security and privacy](https://dl.acm.org/doi/abs/10.1145/3505253.3505260) - A. Suresh, A.A. Saki, M. Alam, R. Onur Topaloglu, S. Ghosh, JETC, 2021  
+ [On quantum obfuscation](https://arxiv.org/abs/1602.01771) - G. Alagic, B. Fefferman  arXiv (preprint),  2016  

<h4 id="measurement-based-quantum-compilation">Measurement-Based Quantum Compilation</h4>

+ [A Generic Measurement-Based Quantum Compilation Pipeline](https://arxiv.org/abs/2302.00795) — Nader M. Mohammadizadeh et al. (2023). 
+ [Adaptive Compilation for Resource-Constrained Photonic One-Way Quantum Computing](https://arxiv.org/abs/2504.17116) — Florian Reiter et al. (2025). 
+ [A Randomness-aware Compiler for Photonic Quantum Computing](https://arxiv.org/abs/2403.01829) — Florian Reiter et al. (2024).
  
</br>
<h2 id="part-d-conference-and-journal">Part D: Conference and Journal</h2>

<h4 id="conference-deadline">Top-tier Conference Deadline</h4>
+ January - [ICCAD](https://www.iccad-conf.com/) 
+ March - [OOPSLA](https://2025.splashcon.org/track/OOPSLA), [TQC](https://tqc-conference.org/)
+ April - [QCE](https://qce.quantum.ieee.org/), [MICRO](https://www.microarch.org/) 
+ August - [ASPLOS](https://www.asplos-conference.org/) <summer cycle>
+ September - [HPCA](https://hpca-conf.org/), [QIP](https://qipconference.org/)
+ November - [CC](https://conf.researchr.org/series/cc) [ISCA](https://iscaconf.org/), [PLDI](https://conf.researchr.org/series/pldi), [DAC](https://www.dac.com/), [CGO](https://2026.cgo.org/) 

**
CCS(Conference on Computer and Communications Security
STOC(ACM Symposium on Theory of Computing)
JETC(ACM Journal on Emerging Technologies in Computing Systems)
**

<h4 id="journals">Journals</h4>
Impact Factor > 10
+ [Nature](https://www.nature.com/)
+ [Science](https://www.science.org/journal/science)
+ [Nature Physics](https://www.nature.com/nphys)  
+ [Nature Communications](https://www.nature.com/ncomms)
+ [PRX Quantum](https://journals.aps.org/prxquantum) 
Impact Factor > 3
+ [npj Quantum Information](https://www.nature.com/npjqi)
+ [ACM TQC](https://dl.acm.org/journal/tqc)
+ [Quantum](https://quantum-journal.org/)
+ [Quantum Science and Technology(QST)](https://iopscience.iop.org/journal/2058-9565)
+ [Quantum Machine Intelligence(QMI)](https://link.springer.com/journal/42484) 
+ [Advanced Quantum Technology(AQT)](https://onlinelibrary.wiley.com/journal/2511902X)

  



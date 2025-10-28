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
  - [Quantum Debugging](#quantum-debugging)
  - [Quantum Formal Verification](#quantum-formal-verification)
  - [QEC-aware Compilation](#qec-aware-compilation)
  - [Quantum Secure Compilation](#quantum-secure-compilation)
- [Part C: Quantum Compiler Niche Fields](#part-c-quantum-compiler-niche-fields)
  - [Topological Quantum Compilation](#topological-quantum-compilation)
  - [Qudit Compilation](#qudit-compilation)
  - [Quantum Circuit Obfuscation](#quantum-circuit-obfuscation)
  - [Measurement-Based Quantum Compilation](#measurement-based-quantum-compilation)
- [Part D: Quantum Study Resource](#part-d-quantum-study-resource)  
  - [Tech blogs](#tech-blogs)
  - [Books](#books)
  - [Blogs of Luminaries](#blogs-of-luminaries)
  - [Conference Deadline From January to December](#conference-deadline)
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
+ [LinguaQuanta: Towards a Quantum Transpiler Between OpenQASM and Quipper](https://arxiv.org/pdf/2404.08147) - Scott Wesley et al., 2024  - [GitHub](https://github.com/onestruggler/qasm-quipper)  
+ [Design and synthesis of scalable quantum programs](https://arxiv.org/abs/2412.07372) - Tomer Goldfriend et al., 2025
+ [PHOENIX: Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) - Zhaohui Yang et al., 2025  - [GitHub](https://github.com/iqubit-org/phoenix)  
+ [Practical and efficient quantum circuit synthesis and transpiling with Reinforcement Learning](https://arxiv.org/abs/2405.13196) - David Kremer et al., 2025  - [GitHub](https://github.com/Qiskit/qiskit-ibm-transpiler)  
+ [Qmod: Expressive High-Level Quantum Modeling](https://arxiv.org/html/2502.19368v1) - Matan Vax et al., 2025  - [GitHub](https://github.com/Classiq/classiq-library)  
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) - David Ittah et al., 2021  - [GitHub](https://github.com/dime10/QIRO)  
+ [A Cross-Platform Execution Engine for the Quantum Intermediate Representation](https://arxiv.org/pdf/2404.14299) - Elaine Wong et al., 2024  - [GitHub](https://github.com/ORNL-QCI/qiree)  
+ [InQuIR: Intermediate Representation for Interconnected Quantum Computers](https://arxiv.org/abs/2302.00267) - Shin Nishio, Ryo Wakizaka, 2023  - [GitHub](https://github.com/team-InQuIR/InQuIR)  
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) - Anurudh Peduri, Siddharth Bhat, CC 2022  - [GitHub](https://github.com/opencompl/QMLIR)  
+ [Quantum circuit transformations with a multi-level intermediate representation compiler](https://arxiv.org/abs/2112.10677) - T. Nguyen et al., 2021
+ [Enabling Retargetable Optimizing Compilers for Quantum Accelerators via a Multi-Level Intermediate Representation](https://arxiv.org/abs/2109.00506) - Thien Nguyen, Alexander McCaskey, 2021
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) - Alexander McCaskey, Thien Nguyen, QCE 2021
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) - Ali JavadiAbhari et al., 2014  - [GitHub](https://github.com/epiqc/ScaffCC)  
+ [Introducing Quantum Intermediate Representation (QIR)](https://devblogs.microsoft.com/qsharp/introducing-quantum-intermediate-representation-qir/)  - [GitHub](https://github.com/qir-alliance/qir-spec)  
</br>

> Loop & Control-Flow Transforms 
+ [Thoughts on Adopting the Quantum Intermediate Representation (QIR)](https://arxiv.org/pdf/2411.18682) – Ynnick Stade et al., 2024
+ [The Limits of Control Flow in Quantum Programming](https://arxiv.org/abs/2304.15000) – Charles Yuan et al., 2023
+ [Software Pipelining for Quantum Loop Programs](https://arxiv.org/abs/2012.12700) – Jingzhe Guo, Mingsheng Ying, IEEE TSE 2023
+ [Exploring the Impact of Affine Loop Transformations in Qubit Allocation](https://arxiv.org/pdf/2010.11999) – Martin Kong, 2020
</br>

> Quantum Circuit Analysis 
+ [Character Complexity: A Novel Measure for Quantum Circuit Analysis](https://arxiv.org/abs/2408.09641) - Daksh Shami, 2024
+ [QuCT: A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) - Siwei Tan et al., MICRO 2023  - [GitHub](https://github.com/JanusQ/QuCT-Micro2023) 
+ [Quantum Vulnerability Analysis to Guide Robust Quantum Computing System Design](https://arxiv.org/pdf/2207.14446) - Fang Qi et al., 2023
</br>


<h4 id="hardware-agnostic-optimization">Hardware-Agnostic Optimization</h4>

> Quantum Program Optimization 
+ [SuperstaQ: Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) - Campbell et al., QCE 2023  - [GitHub](https://github.com/Infleqtion/client-superstaq)  
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


> Circuit Transformation 
+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) - Francesco Preti,. Quantum, 2024
+ [Geyser: a compilation framework for quantum computing with neutral atoms](https://dl.acm.org/doi/abs/10.1145/3470496.3527428) - T. Patel et al., ISCA, 2022
+ [Backend compiler phases for trapped-ion quantum computers](https://arxiv.org/abs/2206.00544) - T. Schmale et al., 2022
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) - Fabian Kreppel et al., 2022

> Circuit Optimisation 
+ [A Resource-Allocating Compiler for Lattice Surgery](https://arxiv.org/abs/2506.04620) - Alan Robertson, Haowen Gao, Yuval R. Sanders, 2025.  - [GitHub](https://github.com/latticesurgery-com/lattice-surgery-compiler)  
+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) - Francisco J. R. Ruiz, Nature Machine Intelligence, 2025.  - [GitHub](https://github.com/google-deepmind/alphatensor_quantum)  
+ [Q-Pilot: Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) - Hanrui Wang., DAC, 2024.
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) - Jonathan Durandau, Quantum, 2023.  - [GitHub](https://github.com/cda-tum/mqt-ion-shuttler)  [oai_citation:2‡GitHub](https://github.com/cda-tum/mqt-ion-shuttler?utm_source=chatgpt.com)
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) - S. Ebadi et al., Science, 2022.  - [GitHub](https://github.com/QuEraComputing/Bloqade.jl)  
+ [Full-stack quantum computing systems in the NISQ era: algorithm-driven and hardware-aware compilation techniques](https://arxiv.org/abs/2204.06369) - Mendina Bandic, DATE, 2022.
+ [Software-hardware co-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - Gushu Li et al., ISCA, 2021.
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) - Zikun Li et al., OOPSLA, 2024.  - [GitHub](https://github.com/quantum-compiler/Quarl) 
+ [Machine Learning Optimization of Quantum Circuit Layouts](https://dl.acm.org/doi/full/10.1145/3565271) - Alexandru Pale et al., ACM TQC, 2023.  - [GitHub](https://github.com/alexandrupaler/qxx)  
+ [Synthesizing Quantum-Circuit Optimizers](https://dl.acm.org/doi/abs/10.1145/3591254) - Amanda Xu et al., PLDI, 2023.  - [GitHub](https://github.com/qqq-wisc/queso)
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) - Bodo Rosenhahn, Tobias J. Osborne, 2023
</br>



<h4 id="hardware-aware-compilation-mapping">Hardware-Aware Compilation & Mapping</h4>

+ [Short Two-Qubit Pulse Sequences for Exchange-Only Spin Qubits in 2D Layouts](https://arxiv.org/abs/2412.14918) - Jason D. Chadwick et al., 2025
+ [CCMap: Hardware-Aware Compilation for Chip-to-Chip Coupler-Connected QPUs](https://arxiv.org/abs/2505.09036) - Zefan Du et al., 2025
+ [Virtual-Z Gates and Symmetric Gate Compilation](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.020348) - Arian Vezvaee et al., 2025
+ [Selective Excitation of Superconducting Qubits with a Shared Control Line through Pulse Shaping](https://arxiv.org/pdf/2501.10710) - Ryo Matsuda et al., 2025
+ [Short Two-Qubit Pulse Sequences for Exchange-Only Spin Qubits](https://arxiv.org/html/2412.14918v3) - Jason D. Chadwick et al., 2025
+ [CCMap: Hardware-Aware Compilation for Chip-to-Chip Coupler-Connected QPUs](https://arxiv.org/abs/2505.09036) - Zefan Du et al., 2025
+ [Qibosoq: RFSoC Control Software for Self-Hosted Quantum Hardware via QICK](https://arxiv.org/abs/2310.05851) - Andrea Pasquale et al., 2025  - [GitHub](https://github.com/qiboteam/qibosoq)  
+ [QUAlibrate: Open-Source Framework that Cuts Calibration from Hours to Minutes](https://www.prnewswire.com/il/news-releases/quantum-machines-launches-qualibrate-an-open-source-framework-that-cuts-quantum-computer-calibration-from-hours-to-minutes-302458926.html) - Quantum Machines Team, 2025  - [GitHub](https://github.com/qua-platform/qualibrate)  
+ [Qibolab: An Open-Source Hybrid Quantum Operating System](https://quantum-journal.org/papers/q-2024-02-12-1247/) - Stavros Efthymiou et al., 2024  - [GitHub](https://github.com/qiboteam/qibolab)  
+ [Sensitivity-Adapted Closed-Loop Optimization for High-Fidelity CZ Gates](https://arxiv.org/abs/2412.17454) - Niklas J. Glaser et al., 2024
+ [Pulse Family Optimization for Parametrized Quantum Gates Using Spectral Clustering](https://arxiv.org/abs/2408.00119) - Robert de Keijzer et al., 2024
+ [Graph-Based Pulse Representation for Diverse Quantum Control Hardware](https://arxiv.org/abs/2409.08407) - Aniket S. Dalvi et al., 2024
+ [Pulse-Based Variational Quantum Optimization and Metalearning in Superconducting Circuits](https://arxiv.org/abs/2407.12636) - Yapeng Wang et al., 2024
+ [Implementing Fast and High-Fidelity Quantum Operations Using Open-Loop Optimal Control](https://arxiv.org/abs/2410.22603) - LBNL Collaboration, 2024
+ [Direct Pulse-Level Compilation of Arbitrary Quantum Logic Gates on Superconducting Qutrits](https://arxiv.org/abs/2303.04261) - Yujin Cho et al., 2024
+ [Qibocal: An Open-Source Framework for Calibration of Self-Hosted Quantum Devices](https://arxiv.org/abs/2410.00101) - Andrea Pasquale et al., 2024  - [GitHub](https://github.com/qiboteam/qibocal) 
+ [A Time-Optimisation Framework Enabling Fast and Robust Gates in One Circuit](https://arxiv.org/pdf/2412.18533) - Eduardo W. Lussi et al., 2024
+ [A Time Optimization Framework for Robust and Low-Latency Quantum Circuits](https://arxiv.org/abs/2412.18533) - Eduardo W. Lussi et al., 2024
+ [Qibolab: Pulse-Oriented Drivers for Custom Hardware](https://quantum-journal.org/papers/q-2024-02-12-1247/) - Stavros Efthymiou et al., 2024  - [GitHub](https://github.com/qiboteam/qibolab)  
+ [Pulse-Family Optimisation via Spectral Clustering](https://arxiv.org/abs/2408.00119) - Robert de Keijzer et al., 2024
</br>

> Circuit Scheduling 
+ [Quantum circuit scheduler for QPUs usage optimization](https://arxiv.org/html/2404.01055v1) - Javier Romero-Alvarez et al., 2024.  - [GitHub](https://github.com/Qcraft-UEx/QCRAFT-AutoScheduler)  
+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) - Toshinari Itoko, Takashi Imamichi, QCE, 2020
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) - Gian Giacomo Guerreschi, Jongsoo Park, Quantum Sci, 2017
</br>

> Qubit Mapping & Routing 
+ [S-SYNC: Shuttle & SWAP Co-Optimisation in QCCD](https://arxiv.org/abs/2505.01316) - Chenghong Zhu, Xian Wu, Jingbo Wang, Xin Wang, ISCA 2025
+ [Compiling quantum circuits for dynamically field-programmable neutral atoms array processors](https://arxiv.org/pdf/2306.03487.pdf) - D. B. Tan et al., 2024
+ [Qubit mapping for reconfigurable atom arrays](https://dl.acm.org/doi/abs/10.1145/3508352.3549331) - B. Tan et al, ICCAD, 2022
+ [Qubit Mapping Toward Quantum Advantage](https://arxiv.org/pdf/2210.01306v1.pdf) - Chin-Yi Cheng et al., 2022
+ [Qubit Mapping and Routing via MaxSAT](https://arxiv.org/abs/2208.13679v1) - Abtin Molavi, Amanda Xu, Martin Diges, Lauren Pick, Swamit Tannu, Aws Albarghouthi, MICRO, 2022
+ [QuCloud: A New Qubit Mapping Mechanism for Multi-programming Quantum Computing in Cloud Environment](https://ieeexplore.ieee.org/document/9407180) - Lei Liu, Xinglei Dou, HPCA, 2021
+ [Optimal mapping for near-term quantum architectures based on Rydberg atoms](https://arxiv.org/abs/2109.04179) - S.Brandhofer et al., ICCAD, 2021
+ [Time-optimal Qubit mapping](https://dl.acm.org/doi/pdf/10.1145/3445814.3446706) - Chi Zhang et al., ASPLOS, 2021
+ [Not All Qubits Are Created Equal: A Case for Variability-Aware Policies for NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007) - Swamit S. Tannu, Moinuddin K. Qureshi, ASPLOS, 2019
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/1901.11054) - Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi, ASPLOS, 19
+ [Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.](https://arxiv.org/abs/1901.11054) - Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi, ASPLOS, 2019
</br>

<h4 id="pulse-level-compilation-control">Pulse-Level Compilation & Control</h4>

+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) - Philipp Seitz et al., Quantum Week, 2024.  - [GitHub](https://github.com/qc-tum/milq)  
+ [DISQ: Dynamic Iteration Skipping for Variational Quantum Algorithms](https://arxiv.org/abs/2308.06634) - Junyao Zhang et al., QCE, 2023
+ [Let Each Quantum Bit Choose Its Basis Gates](https://arxiv.org/abs/2208.13380) - Sophia Fuhui Lin et al., MICRO, 2022
+ [Software-hardware co-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - Gushu Li et al., ISCA 2021
+ [Error Mitigation in Quantum Computers through Instruction Scheduling](https://arxiv.org/abs/2105.01760) - Kaitlin N. Smith et al., 2021.
+ [EQC: ensembled quantum computing for variational quantum algorithms](https://arxiv.org/abs/2111.14940) - Samuel Stein et al., ISCA, 2022.  - [GitHub](https://github.com/pnnl/eqc)  
+ [Software mitigation of crosstalk on noisy intermediate-scale quantum computers](https://arxiv.org/abs/2001.02826) - Prakash Murali et al., ASPLOS, 2020.
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/abs/2010.15876) - Xin-Chuan Wu et al., HPCA, 2020
</br>

<h4 id="runtime-dynamic-execution">Runtime & Dynamic Execution</h4>

+ [Extending the OmpSs-2 Programming Model for Hybrid Quantum-Classical Programming](https://arxiv.org/abs/2502.21104) - Philip Döbler et al., 2025  - [GitHub](https://github.com/bsc-pm/ompss-2-releases) 
+ [Qibosoq: RFSoC Control Software for Self-Hosted Quantum Hardware via QICK](https://cds.cern.ch/record/2875598) - Andrea Pasquale et al., 2025  - [GitHub](https://github.com/qiboteam/qibosoq)  
+ [Building a Software Stack for Quantum-HPC Integration](https://arxiv.org/abs/2503.01787) - Amir Shehata et al., 2025
+ [SLURM Heterogeneous Jobs for Hybrid Classical-Quantum Workflows](https://arxiv.org/abs/2506.03846) - Aniello Esposito & Utz-Uwe Haus, 2025
+ [phase2: Full-State Vector Simulation of Quantum Time Evolution at Scale](https://doi.org/10.21203/rs.3.rs-6620681/v1) - Marek Miller et al., 2025  - [GitHub](https://github.com/Quantum-for-Life/phase2) 
+ [Realization of Constant-Depth Fan-Out with Real-Time Feed-forward on a Superconducting Processor](https://arxiv.org/abs/2409.06989) - Yongxin Song et al., 2024
+ [Demonstrating Real-Time & Low-Latency Quantum Error Correction](https://arxiv.org/abs/2410.05202) - Laura Caune et al., 2024
+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) - Philipp Seitz et al., 2024  - [GitHub](https://github.com/qc-tum/milq) 
+ [Qibolab: An Open-Source Hybrid Quantum Operating System](https://quantum-journal.org/papers/q-2024-02-12-1247/) - Stavros Efthymiou et al., 2024  - [GitHub](https://github.com/qiboteam/qibolab)  
+ [Multi-GPU-Enabled Hybrid Quantum-Classical Workflow in Quantum-HPC Middleware](https://arxiv.org/abs/2403.05828) - Kuan-Cheng Chen et al., 2024  - [GitHub](https://github.com/Louisanity/cuPhastLearn) 
+ [Combining Quantum Processors with Real-Time Classical Communication](https://www.nature.com/articles/s41586-024-08178-2) - Almudena Carrera Vazquez et al., Nature, 2024. - [GitHub](https://github.com/eggerdj/cut_graph_state_data) 
+ [Pilot-Quantum: A Middleware for Quantum-HPC Resource & Task Management](https://arxiv.org/abs/2412.18519) - Pradeep Mantha et al., 2024  - [GitHub](https://github.com/radical-cybertools/pilot-quantum)  
+ [A Pragma-Based C++ Framework for Hybrid Quantum / Classical Computation](https://arxiv.org/abs/2309.02605) - Agnieszka Gazda et al., 2024
+ [Scaling Quantum Computing with Dynamic Circuits](https://arxiv.org/abs/2402.17833) - Almudena Carrera Vazquez et al., 2024
+ [Energy Efficiency of Quantum State-Vector Simulation at Scale](https://arxiv.org/pdf/2308.07402) - Jakub Adamski et al., 2023  - [GitHub](https://github.com/jjacobx/arb23) 

<h2 id="part-b-quantum-compiler-ecosystem">Part B: Quantum Compiler Ecosystem</h2>

<h4 id="quantum-debugging">Quantum Debugging</h4>

+ [Quito: A Framework for Testing Quantum Programs](https://dl.acm.org/doi/10.1145/3428219.3428260) — Y. Long, L. Zhao (2020). Proceedings of the ACM on Programming Languages (OOPSLA)
+ [QuraTest: Automated Testing of Quantum Programs with Complex Input States](https://dl.acm.org/doi/10.1109/ASE56229.2023.00196) — J. Ye, et al. (2023). IEEE Transactions on Quantum Engineering
+ [QOPS: Quantum Oracle Property Specification for Testing Quantum Programs](https://dl.acm.org/doi/10.1145/3691620.3695275) — J. Ye, et al. (2022). Proceedings of the 44th International Conference on Software Engineering (ICSE)
+ [Muskit: Mutation Testing for Qiskit Quantum Programs](https://ieeexplore.ieee.org/document/9678563) — A. Mendiluze, et al. (2021). Proceedings of the 43rd International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP)
+ [QMutPy: Mutation Testing Framework for Quantum Programs](https://jose.github.io/assets/pdfs/ISSTA2022-tool-paper.pdf) — E. Fortunato, et al. (2022). Proceedings of the 37th IEEE/ACM International Conference on Automated Software Engineering (ASE)
+ [MorphQ: Metamorphic Testing for Quantum Programs](https://arxiv.org/abs/2206.01111) — M. Paltenghi, M. Pradel (2023). Proceedings of the 45th International Conference on Software Engineering (ICSE)
+ [QuSBT: Search-Based Testing of Quantum Programs](https://dl.acm.org/doi/10.1145/3510454.3516839) — Y. Long, L. Zhao (2021). Empirical Software Engineering
+ [QuCAT: Quantum Combinatorial Testing Framework](https://arxiv.org/abs/2309.00119) — Y. Long, L. Zhao (2020). Proceedings of the 35th IEEE/ACM International Conference on Automated Software Engineering (ASE)
+ [Statistical Assertions for Quantum Programs](https://arxiv.org/abs/2507.16255) — H.-L. Huang, M. Martonosi (2017). Proceedings of the 39th International Conference on Software Engineering (ICSE)
+ [Runtime Assertions for Quantum Programs](https://arxiv.org/abs/2506.18458) — J. Liu, et al. (2021). Proceedings of the 43rd International Conference on Software Engineering (ICSE)
+ [Swap-Based Assertions for Quantum Programs](https://hzhou.wordpress.ncsu.edu/files/2022/12/hpca21.pdf) — J. Liu, H. Zhou (2022). IEEE Transactions on Quantum Engineering
+ [Assertions for Symmetry States in Quantum Circuits](https://arxiv.org/abs/2507.16255) — Y. Li, et al. (2023). Proceedings of the 60th Annual Design Automation Conference (DAC)
+ [QuAssert: Automated Assertion Generation for Quantum Programs](https://arxiv.org/abs/2303.01487) — Y. Li, et al. (2024). Proceedings of the 46th International Conference on Software Engineering (ICSE)
+ [QDebug: Debugging Quantum Programs with Probabilistic Cloning](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4511772) — T. Sato, et al. (2022). Proceedings of the 44th International Conference on Software Engineering (ICSE)
+ [Cirquo: Slicing-Based Debugging for Quantum Circuits](https://arxiv.org/abs/2205.01899) — Z. Metwalli, R. Van Meter (2021). Proceedings of the 43rd International Conference on Software Engineering (ICSE)

<h4 id="quantum-formal-verification">Quantum Formal Verification</h4>

+ [CoqQ: Foundational Verification of Quantum Programs](https://arxiv.org/abs/2207.11350) — L. Zhou, G. Barthe, P.-Y. Strub, J. Liu, M. Ying (2022). 
+ [Twist: Sound Reasoning for Purity and Entanglement in Quantum Programs](https://arxiv.org/abs/2205.02287) — C. Yuan, C. McNally, M. Carbin (2022). Proceedings of the ACM on Programming Languages (POPL)
+ [An Algebraic Method to Fidelity-based Model Checking over Quantum Markov Chains](https://arxiv.org/abs/2101.04971) — M. Xu, J. Fu, J. Mei, Y. Deng (2021). 
+ [CertiQ: A Mostly-automated Verification of a Realistic Quantum Compiler](https://arxiv.org/pdf/1908.08963) — Y. Shi, R. Tao, X. Li, A. Javadi-Abhari, A. W. Cross, F. T. Chong, R. Gu (2020).  
+ [Quantum Relational Hoare Logic](https://arxiv.org/abs/1802.03188) — D. Unruh (2019). Proceedings of the ACM on Programming Languages (POPL)
+ [Quantum Temporal Logic](https://arxiv.org/abs/1908.00158) — N. Yu (2019). 
+ [ProbReach: Verified Probabilistic Delta-Reachability for Stochastic Hybrid Systems](https://arxiv.org/abs/1410.8060) — F. Shmarov, P. Zuliani (2015). (HSCC)
+ [Formal Verification of Quantum Algorithms Using Quantum Hoare Logic](https://link.springer.com/chapter/10.1007/978-3-030-25543-5_12) — J. Liu, B. Zhan, S. Wang, S. Ying, T. Liu, Y. Li, M. Ying, N. Zhan (2019). Computer Aided Verification (CAV)
+ [Quantum relational Hoare logic](https://dl.acm.org/doi/10.1145/3290346) — J. Liu, B. Zhan, S. Wang, S. Ying, T. Liu, Y. Li, M. Ying, N. Zhan (2019). (POPL)
+ [Model Checking Quantum Systems — A Survey](https://arxiv.org/abs/1807.09466) — M. Ying, Y. Feng, R. Duan, Z. Ji (2018).
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
+ [Analyzing Strategies for Dynamical Decoupling Insertion on IBM Quantum](https://arxiv.org/abs/2204.14251), Murphy Y. Niu & Daniel A. Lidar, arXiv, 2022
+ [Qubit Mapping and Routing via MaxSAT](https://pages.cs.wisc.edu/~amolavi/files/micro22.pdf), Maryam Amiri et al., MICRO, 2022.
+ [VAQEM: A Variational Approach to Quantum Error Mitigation](https://www.computer.org/csdl/proceedings-article/hpca/2022/202700a288/1Ds0fvoYbCw) - Gokul S. Ravi et al., HPCA, 2022
+ [Exploiting Long-Distance Interactions and Tolerating Atom Loss in Neutral Atom Quantum Architectures](https://arxiv.org/pdf/2111.06469.pdf) - Jonathan M. Baker, et al., ISCA, 2021
+ [ADAPT: Mitigating Idling Errors in Qubits via Adaptive Dynamical Decoupling](https://dl.acm.org/doi/10.1145/3466752.3480059) - Poulami Das et al., MICRO, 2021
+ [A Noise-Aware Qubit Mapping Algorithm Evaluated via Qubit Interaction-Graph Criteria](https://www.researchgate.net/publication/350512755_A_Noise-Aware_Qubit_Mapping_Algorithm_Evaluated_via_Qubit_Interaction-Graph_Criteria) - Matthew Steinberg et al., arXiv, 2021.
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) - Xin-Chuan Wu, Dripto M Debroy, Yongshan Ding, Jonathan M Baker, Yuri Alexeev, Kenneth R Brown, and Frederic T Chong, HPCA, 2020
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503), Yongshan Ding, Pranav Gokhale, Sophia Fuhui Lin, Richard Rines, Thomas Propson, Frederic T. Chong, MICRO, 2020
+ [Digital Zero-Noise Extrapolation for Quantum Error Mitigation](https://arxiv.org/abs/2005.10921), Tudor Giurgica-Tiron et al., IEEE QCE, 2020 
+ [Noise-Adaptive Compiler Mappings for NISQ Computers](https://dl.acm.org/doi/10.1145/3297858.3304075), Prakash Murali et al., ASPLOS, 2019
+ [Near-Optimal Routing of Noisy Quantum States](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/11134/111340A/Near-optimal-routing-of-noisy-quantum-states/10.1117/12.2526670.short), Kyle Cote et al., SPIE Proc., 2019.
+ [Not All Qubits Are Created Equal: Variation-Aware Qubit Allocation in NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007), Swamit Tannu & Moinuddin Qureshi, ASPLOS, 2019
+ [Practical Quantum Error Mitigation for Near-Future Applications](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509), Suguru Endo et al., Phys. Rev. X, 2018.  
+ [Error Mitigation for Short-Depth Quantum Circuits](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509), Kristan Temme et al., Phys. Rev. Lett., 2017.
</br>



<h4 id="quantum-secure-compilation">Quantum Secure Compilation</h4>

+ [Split Compilation for Security of Quantum Circuits](https://pure.psu.edu/en/publications/split-compilation-for-security-of-quantum-circuits) — Abdullah Ash Saki, Aakarshitha Suresh, Rasit Onur Topaloglu, Swaroop Ghosh. ICCAD 2021.  ￼
+ [A Quantum Circuit Obfuscation Methodology for Security and Privacy](https://arxiv.org/abs/2104.05943) — Aakarshitha Suresh, Abdullah Ash Saki, Mahabubul Alam, Rasit Onur Topaloglu, Swaroop Ghosh. HASP @ MICRO 2021.  ￼
+ [OpaQue: Program Output Obfuscation for Quantum Software Circuits in Quantum Clouds](https://hpcrl.github.io/ICS2025-webpage/program/Proceedings_ICS25/ics25-32.pdf) — Tirthak Patel, Aditya Ranjan, Daniel Silver, Harshitta Gandhi, William Cutler, Devesh Tiwari. ICS 2025.  ￼
+ [TetrisLock: Quantum Circuit Split Compilation with Interlocking Patterns](https://arxiv.org/abs/2503.11982) — Qian Wang, Jayden John, Ben Dong, Yuntao Liu. arXiv 2025 (preprint).  ￼
+ [OPAQUE: Obfuscating Phase in Quantum Circuit Compilation for Efficient IP Protection](https://www.arxiv.org/abs/2502.16605) — Anees Rehman, Vincent Langford, Yuntao Liu. ISQED 2025.  ￼
+ [Encrypted-state quantum compilation scheme based on quantum circuit obfuscation](https://arxiv.org/abs/2507.17589) (ECQCO) — Chenyi Zhang, Tao Shang, Xueyi Guo, Yuanjing Zhang. arXiv 2025.  ￼
+ [Classical Obfuscation of Quantum Circuits via Publicly-Verifiable QFHE](https://arxiv.org/abs/2510.08400) — James Bartusek, Aparna Gupte, Saachi Mutreja, Omri Shmueli. arXiv 2025 (preprint).  ￼
+ [Quantum Homomorphic Encryption for Circuits of Low T-gate Complexity](https://link.springer.com/chapter/10.1007/978-3-662-48000-7_30) — Anne Broadbent, Stacey Jeffery. CRYPTO 2015.  ￼
+ [Unconditionally Verifiable Blind Quantum Computation](https://journals.aps.org/pra/pdf/10.1103/PhysRevA.96.012303) — Joseph F. Fitzsimons, Elham Kashefi. Physical Review A, 2017. 


<h2 id="part-c-quantum-compiler-niche-fields">Part C: Quantum Compiler Niche Fields</h2>

<h4 id="topological-quantum-compilation">Topological Quantum Compilation</h4>

+ [Topological quantum compilation of two-qubit gates](https://arxiv.org/abs/2408.07132) — Parsa Hosseini et al. (2024). 
+ [Topological quantum compilation of metaplectic anyons based on the genetic optimized algorithms](https://arxiv.org/abs/2501.01745) — Parsa Hosseini et al. (2025). 
+ [Optimized Topological Quantum Compilation of Three-Qubit Controlled Gates in the Fibonacci Anyon Model](https://arxiv.org/abs/2311.17645) — Parsa Hosseini et al. (2023). 
+ [Asymptotically Optimal Topological Quantum Compiling](https://arxiv.org/abs/1310.4150) — Michael Freedman et al. (2013). 
+ [Provably Optimal Quantum Circuits with Mixed-Integer Programming](https://arxiv.org/abs/2510.00649) — Yufei Ding et al. (2025). 


<h4 id="qudit-compilation">Qudit Compilation</h4>

+ [Efficient, direct compilation of SU(N) operations into SNAP](https://arxiv.org/abs/2307.11900) — Vladislav D. Kurpas et al. (2023). 
+ [QudCom: Towards Quantum Compilation for Qudit Systems](https://arxiv.org/abs/2311.07015) — Sebastian Brandhofer et al. (2023). 
+ [Adaptive Compilation of Multi-Level Quantum Operations](https://arxiv.org/abs/2206.03842) — David R. M. Arvidsson-Shukur et al. (2022). 
+ [Compilation of Entangling Gates for High-Dimensional Quantum Processors](https://arxiv.org/abs/2301.04155) — Manuel G. J. B. A. Cordier et al. (2023). 
+ [MQT Qudits: A Software Framework for Mixed-Dimensional Quantum Computing](https://arxiv.org/abs/2410.02854) — Lukas Burgholzer et al. (2024). 

<h4 id="quantum-circuit-obfuscation">Quantum Circuit Obfuscation</h4>

+ [Quantum state obfuscation from classical oracles](https://dl.acm.org/doi/abs/10.1145/3618260.3649673) - J. Bartusek, Z. Brakerski, V. Vaikuntanathan, ACM Conference on Computer and Communications Security (CCS), 2024
+ [Obfuscation of pseudo-deterministic quantum circuits](https://dl.acm.org/doi/abs/10.1145/3564246.3585179) - J. Bartusek, F. Kitagawa, R. Nishimaki, ACM Symposium on Theory of Computing (STOC), 2023  
+ [Indistinguishability obfuscation of null quantum circuits and applications](https://arxiv.org/abs/2106.06094) - J. Bartusek, G. Malavolta, arXiv (preprint), 2021
+ [A quantum circuit obfuscation methodology for security and privacy](https://dl.acm.org/doi/abs/10.1145/3505253.3505260) - A. Suresh, A.A. Saki, M. Alam, R. Onur Topaloglu, S. Ghosh, ACM Journal on Emerging Technologies in Computing Systems, 2021  
+ [On quantum obfuscation](https://arxiv.org/abs/1602.01771) - G. Alagic, B. Fefferman  arXiv (preprint),  2016  

<h4 id="measurement-based-quantum-compilation">Measurement-Based Quantum Compilation</h4>

+ [A Generic Measurement-Based Quantum Compilation Pipeline](https://arxiv.org/abs/2302.00795) — Nader M. Mohammadizadeh et al. (2023). 
+ [Adaptive Compilation for Resource-Constrained Photonic One-Way Quantum Computing](https://arxiv.org/abs/2504.17116) — Florian Reiter et al. (2025). 
+ [A Randomness-aware Compiler for Photonic Quantum Computing](https://arxiv.org/abs/2403.01829) — Florian Reiter et al. (2024). 
+ [Topological Quantum Gates in Homotopy Type Theory](https://arxiv.org/abs/2303.02382) — Guillaume Munch-Madewig et al. (2023). 
+ [Systematic Computation of Braid Generator Matrix in Topological Quantum Computation](https://arxiv.org/abs/2307.01892) — Parsa Hosseini et al. (2023). 


<h2 id="part-d-quantum-study-resource">Part D: Quantum-Study-Resource</h2>

<h4 id="tech blogs">Tech Blogs</h4>

+ [TKET Developer Blog (Quantinuum)](https://docs.quantinuum.com/tket/blog/) - Updates on optimizer passes, SWAP-routing & new ISA back-ends.    
+ [Classiq Insights](https://www.classiq.io/insights) - Posts on high-level synthesis and automatic circuit generation.   
+ [AWS Quantum Technologies Blog](https://aws.amazon.com/blogs/quantum-computing/) - Notes on parametric compilation & hybrid-runtime transpilation.  
+ [Q-CTRL Blog](https://q-ctrl.com/blog) - Pulse-level scheduling, error-robust instruction sets & control-compiler tricks.  
+ [Rigetti Tech Blog](https://medium.com/rigetti) - Quil-C compiler upgrades and hybrid workflow engineering.    
+ [IBM Quantum Blog](https://www.ibm.com/quantum/blog) - Transpiler roadmaps, dynamic circuits & Qiskit optimization updates.    
+ [Microsoft Blog – Introducing QIR](https://quantum.microsoft.com/en-us/insights/blogs/qir/introducing-quantum-intermediate-representation-qir) - Design rationale & evolution of the QIR stack.  
+ [Zapata Orquestra Feature](https://www.hpcwire.com/2022/07/28/zapatas-orquestra-targets-the-hybrid-quantum-classical-challenge/) - Workflow compiler orchestrating hybrid quantum–classical pipelines.   
+ [PsiQuantum Newsroom](https://www.psiquantum.com/news) - Photonic-specific compilation & mapping announcements (Omega chipset).  
+ [Quantum Circuits × NVIDIA Partnership](https://quantumcircuits.com/key-partnership-with-nvidia/) - CUDA-Q compiler integration for error-aware superconducting qubits. 

<h4 id="books">Books</h4>

+ [Quantum Computer Systems: Research for Noisy Intermediate-Scale Quantum Computers](https://www.amazon.co.uk/Quantum-Computer-Synthesis-Lectures-Architecture/dp/168173866X) – NISQ-era architecture/​compiler co-design guide.  
+ [Quantum Computing for Computer Architects, 2e](https://link.springer.com/book/10.1007/978-3-031-01731-5) 
+ [Programming Quantum Computers](https://www.oreilly.com/library/view/programming-quantum-computers/9781492039673/) 
+ [Quantum Computing: An Applied Approach, 2e](https://link.springer.com/book/10.1007/978-3-030-83274-2) 



<h4 id="blogs of luminaries">Blogs of Luminaries</h4>

+ [Scott Aaronson](https://scottaaronson.blog/) 
+ [John Preskill](https://quantumfrontiers.com/)  
+ [Dave Bacon](https://dabacon.org/pontiff/) 
+ [Gil Kalai](https://gilkalai.wordpress.com/) 
+ [Michael Nielsen](https://michaelnielsen.org/blog/)   
+ [John C. Baez](https://johncarlosbaez.wordpress.com/)
+ [Robert Harper](https://existentialtype.wordpress.com/)
+ [Chris Lattner](https://www.nondot.org/sabre/)

<h4 id="conference-deadline">Conference Deadline From January to December</h4>

+ [CF](https://www.computingfrontiers.org/) - Late Jan
+ [IQSOFT](https://iqsoft.scitevents.org/) - Mid Fed
+ [IEEE QSW](https://services.conferences.computer.org/2025/qsw/) - Early Mar [ASPLOS](https://www.asplos-conference.org/) - Early Mar [QPL](https://qpl2025.github.io/) - Early Mar [TQC](https://tqc-conference.org/) - Early Mar
+ [QCE](https://qce.quantum.ieee.org/) - Mid April [MICRO](https://www.microarch.org/) - Mid April [ICCAD](https://iccad.com/) - Mid April
+ [HPCA](https://hpca-conf.org/) - Mid Sep [QIP](https://qipconference.org/) - Mid Sep
+ [CC](https://conf.researchr.org/series/cc) - Early Nov [ISCA](https://iscaconf.org/) - Mid Nov [PLDI](https://conf.researchr.org/series/pldi) - Mid Nov [DAC](https://www.dac.com/) - Mid Nov  


<h4 id="journals">Journals</h4>

Impact Factor > 10
+ [Nature](https://www.nature.com/)
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

  



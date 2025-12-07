## Awesome Quantum Compiler
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://GitHub.com/Naereen/ama)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yucheol-choi/)

### Description
As a student researching quantum compilers, I curate influential papers from top conferences and journals. I hope this collection supports your work as much as it supports mine.🙂


## Table of Contents
- [Survey papers](#survey-papers)
- [Part A: Quantum Compilation Pipeline: Algo to Pulse](#part-a-compilation-flow--from-algorithm-to-pulse)
  - [High-Level Languages and Intermediate Representation](#language-logical-ir)
  - [Hardware-Agnostic Optimization](#hardware-agnostic-optimization)
  - [Hardware-Aware Compilation & Mapping](#hardware-aware-compilation--mapping)
  - [Pulse-Level Compilation & Control](#pulse-level-compile)
  - [Runtime & Dynamic Execution](#runtime--dynamic-execution)
- [Part B: Quantum Compiler Ecosystem](#part-b-quantum-compiler-ecosystem)
  - [Quantum Testing and Debugging](#quantum-testing-and-debugging)
  - [Quantum Formal Verification](#quantum-formal-verification)
  - [Lattice Surgery & Surface Code Compilation](#lattice-surgery-surface-code-compilation)
  - [Quantum Circuit Analysis](#quantum-circuit-analysis)
  - [Emerging Topics](#quantum-compiler-emerging-topics)
- [Part C: Quantum Hardware Specific Compilation](#part-c-quantum-hardware-specific-compilation)
  - [Superconducting QC](#superconducting-qc)
  - [Trapped-ion QC](#trapped-ion-qc)
  - [Photonics QC](#photonics-qc)
  - [Neutral-atom QC](#neutral-atom-qc)
  - [Silicon Spin QC](#silicon-spin-qubit-qc)
  - [Topological QC](#topological-qc)
- [Part D: Conference and Journal](#part-d-conference-and-journal) 
  - [Top-tier Conference Deadline](#conference-deadline)
  - [Journals](#journals)
</br>

<h2 id="survey-papers">Survey papers</h2>

+ [Quantum Compilation Process: A Survey](https://link.springer.com/chapter/10.1007/978-3-031-90200-0_9) F. Javier Cardama et al 2025
+ [Quantum Compiler Design for Qubit Mapping and Routing: A Cross-Architectural Survey of Superconducting, Trapped-Ion, and Neutral Atom Systems](https://arxiv.org/pdf/2505.16891) Chenghong zhu et al 2025.
+ [A Comprehensive Review of Quantum Circuit Optimization: Current Trends and Future Directions](https://www.mdpi.com/2624-960X/7/1/2) Krishnageetha Karuppasamy et al 2025.
+ [Quantum Circuit Synthesis and Compilation Optimization: Overview and Prospects](https://arxiv.org/html/2407.00736v1) Ge Yan et al 2024
+ [Quantum Compiling](https://arxiv.org/abs/2112.00187) Marco Maronese 2021

<h2 id="part-a-compilation-flow--from-algorithm-to-pulse">Part A: Quantum Compilation Pipeline: Algo to Pulse</h2>

<h4 id="language-logical-ir">High-Level Language and Logical Intermediate Representation</h4>

> Intermediate Representation and Quantum Transpilation
+ [PHOENIX: Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) Zhaohui Yang et al <img src="https://img.shields.io/badge/DAC-2025-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/iqubit-org/phoenix)  
+ [LinguaQuanta: Towards a Quantum Transpiler Between OpenQASM and Quipper](https://arxiv.org/pdf/2404.08147) Scott Wesley et al <img src="https://img.shields.io/badge/Reversible Computation-2024-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/onestruggler/qasm-quipper)
+ [QASMTrans: A QASM based Quantum Transpiler Framework for NISQ Devices](https://arxiv.org/abs/2308.07581) Fei Hua et al <img src="https://img.shields.io/badge/SC-2023-green.svg" alt="13-pages" align="top">
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) Anurudh Peduri, Siddharth Bhat <img src="https://img.shields.io/badge/CC-2022-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/opencompl/QMLIR)  
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) David Ittah et al <img src="https://img.shields.io/badge/TQC-2022-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/dime10/QIRO)
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) Ali JavadiAbhari et al <img src="https://img.shields.io/badge/Parallel Comput-2022-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/epiqc/ScaffCC) 
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) Alexander McCaskey, Thien Nguyen <img src="https://img.shields.io/badge/QCE-2021-green.svg" alt="13-pages" align="top">
+ [Quantum Circuit Transformations with a Multi-Level Intermediate Representation Compiler](https://arxiv.org/abs/2112.10677) Thien Nguyen et al <img src="https://img.shields.io/badge/Arxiv-2021-green.svg" alt="13-pages" align="top"> 
+ [Programming languages and compiler design for realistic quantum hardware](https://www.nature.com/articles/nature23459) Frederic T. Chong <img src="https://img.shields.io/badge/Nature-2017-green.svg" alt="13-pages" align="top">


> Quantum Loop Optimization and Control Flow Transformation
+ [A Denotational Semantics for Quantum Loops](https://arxiv.org/pdf/2506.23320) Nicola Assolini, Alessandra Di Pierro <img src="https://img.shields.io/badge/PLDI-2025-green.svg" alt="13-pages" align="top">
+ [Efficient Implementation of Quantum Recursive Programs](https://arxiv.org/pdf/2408.10054) Zhicheng Zhang, Mingsheng Ying <img src="https://img.shields.io/badge/PLDI-2025-green.svg" alt="13-pages" align="top">
+ [Quantum Control Machine: The Limits of Control Flow in Quantum Programming](https://arxiv.org/pdf/2304.15000) Charles Yuan et al <img src="https://img.shields.io/badge/OOPSLA-2024-green.svg" alt="13-pages" align="top">
+ [The Limits of Control Flow in Quantum Programming](https://arxiv.org/abs/2304.15000) Charles Yuan et al <img src="https://img.shields.io/badge/OOPSLA-2023-green.svg" alt="13-pages" align="top">
+ [Software Pipelining for Quantum Loop Programs](https://arxiv.org/abs/2012.12700) Jingzhe Guo, Mingsheng Ying <img src="https://img.shields.io/badge/TSE-2023-green.svg" alt="13-pages" align="top">
+ [On the Impact of Affine Loop Transformations in Qubit Allocation](https://arxiv.org/pdf/2010.11999) Martin Kong <img src="https://img.shields.io/badge/TQC-2021-green.svg" alt="13-pages" align="top">
  


<h4 id="hardware-agnostic-optimization">Hardware-Agnostic Optimization</h4>

> Quantum Program Optimization 
+ [SuperstaQ: Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) Campbell et al. <img src="https://img.shields.io/badge/QCE-2023-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/Infleqtion/client-superstaq)
+ [Advances in compilation for quantum hardware -- A demonstration of magic state distillation and repeat-until-success protocols](https://arxiv.org/pdf/2310.12106) Natalie C. Brown et al
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/2109.03371) Gushu Li et al. <img src="https://img.shields.io/badge/ASPLOS-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://youtu.be/lXFVkBlh9_Q?si=y_d4SgUwWQPwerch)
+ [A software methodology for compiling quantum programs](https://arxiv.org/abs/1604.01401) Thomas Häner et al <img src="https://img.shields.io/badge/Quantum Sci-2016-green.svg" alt="13-pages" align="top">
+ [Repeat-until-Success: Non-Deterministic Decomposition of Single-Qubit Unitaries](https://arxiv.org/abs/1311.1074) Adam Paetznick, Krysta Svore <img src="https://img.shields.io/badge/Quantum Information & Computation-2014-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/microsoft/Quantum/tree/main/samples/algorithms/repeat-until-success)  
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/abs/1810.00375) Häner, Hoefler, Troyer <img src="https://img.shields.io/badge/OOPSLA-2013-green.svg" alt="13-pages" align="top"> [Youtube](https://youtu.be/v7PDw-zq_oE?si=qh1JzKWSm-JQ8VcR)

> Circuit Optimisation (ML-based Compile Optimisation)

+ [Optimizing Quantum Circuits, Fast and Slow](https://arxiv.org/pdf/2411.04104) Amanda Xu et al <img src="https://img.shields.io/badge/ASPLOS-2025-green.svg" alt="13-pages" align="top">
+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) Francisco J. R. Ruiz <img src="https://img.shields.io/badge/Nature Machine Intelligence-2025-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/google-deepmind/alphatensor_quantum)
+ [MarQSim: Reconciling Determinism and Randomness in Compiler Optimization for Quantum Simulation](https://arxiv.org/pdf/2408.03429) Xiuqi Cao at el <img src="https://img.shields.io/badge/PLDI-2025-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=PHrpg42LKTk)
+ [Bosehedral: Compiler Optimization for Bosonic Quantum Computing](https://arxiv.org/pdf/2402.02279) Junyu Zhou et al <img src="https://img.shields.io/badge/ISCA-2024-green.svg" alt="13-pages" align="top">
+ [Fermihedral: On the Optimal Compilation for Fermion-to-Qubit Encoding](https://arxiv.org/pdf/2403.17794) Yuhao Liu et al <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=TLhNJRZUeas)
+ [Elivagar: Efficient Quantum Circuit Search for Classification](https://arxiv.org/pdf/2401.09393) Sashwat Anagolum et al <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=Mxkrv7TbQqc)
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) Zikun Li et al <img src="https://img.shields.io/badge/OOPSLA-2024-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/quantum-compiler/Quarl) [Youtube](https://youtu.be/DZjz88yDKC4?si=UTgp_1pQznhfs2Zs)
+ [Machine Learning Optimization of Quantum Circuit Layouts](https://dl.acm.org/doi/full/10.1145/3565271) Alexandru Pale et al <img src="https://img.shields.io/badge/ACM TQC-2023-green.svg" alt="13-pages" align="top">  [GitHub](https://github.com/alexandrupaler/qxx)  
+ [Synthesizing Quantum-Circuit Optimizers](https://dl.acm.org/doi/abs/10.1145/3591254) Amanda Xu et al <img src="https://img.shields.io/badge/PLDI-2023-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/qqq-wisc/queso) [Youtube](https://youtu.be/hwGBeUcHFik?si=ESI7D4bJOiHgZZ1z)
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) Bodo Rosenhahn, Tobias J. Osborne <img src="https://img.shields.io/badge/Physical Review Journal-2023-green.svg" alt="13-pages" align="top">
+ [2QAN: A quantum compiler for 2-local qubit Hamiltonian simulation algorithms](arxiv.org/pdf/2108.02099) Lingling Lao, Dan E. Browne <img src="https://img.shields.io/badge/ISCA-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=rBThLSpNpVU)
+ [A Meet-in-the-Middle Algorithm for Fast Synthesis of Depth-Optimal Quantum Circuits](https://arxiv.org/abs/1206.0758) Matthew Amy et al <img src="https://img.shields.io/badge/IEEE TCAD-2021-green.svg" alt="13-pages" align="top">
+ [Automated optimization of large quantum circuits with continuous parameters](https://arxiv.org/abs/1710.07345) Yunseong Nam et al <img src="https://img.shields.io/badge/npj Quantum Information-2017-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/njross/optimizer)


<h4 id="hardware-aware-compilation-mapping">Hardware-Aware Compilation & Mapping</h4>

> Qubit Allocation
+ [Machine-Learning-Based Qubit Allocation for Error Reduction in Quantum Circuits](https://ieeexplore.ieee.org/document/10209261) Travis LeCompte et al <img src="https://img.shields.io/badge/TQE-2023-green.svg" alt="13-pages" align="top">
+ [Qubit Allocation for Distributed Quantum Computing](https://ieeexplore.ieee.org/document/10228915) Yingling Mao et al <img src="https://img.shields.io/badge/INFOCOM-2023-green.svg" alt="13-pages" align="top">
+ [Qubit Allocation](https://hal.science/hal-01655951/file/Siraichi_QubitAllocation_CGO18.pdf) Marcos Siraichi et al <img src="https://img.shields.io/badge/CGO-2018-green.svg" alt="13-pages" align="top">

> Qubit Mapping 
+ [S-SYNC: Shuttle & SWAP Co-Optimisation in QCCD](https://arxiv.org/abs/2505.01316) Chenghong Zhu et al <img src="https://img.shields.io/badge/ISCA-2025-green.svg" alt="13-pages" align="top">
+ [Compiling quantum circuits for dynamically field-programmable neutral atoms array processors](https://arxiv.org/pdf/2306.03487.pdf) Bochen Tan et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [Quantum Circuit Mapping Based on Incremental and Parallel SAT Solving](https://www.cs.cmu.edu/~mheule/publications/SATmap.pdf) Jiong Yang et al <img src="https://img.shields.io/badge/SAT-2024-green.svg" alt="13-pages" align="top">
+ [Qubit mapping for reconfigurable atom arrays](https://dl.acm.org/doi/abs/10.1145/3508352.3549331) Bochen Tan et al <img src="https://img.shields.io/badge/ICCAD-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://youtu.be/-tr8KtDKKDU?si=l2SwrXNY3KWvLOPz)
+ [Qubit Mapping and Routing via MaxSAT](https://arxiv.org/abs/2208.13679v1) Abtin Molavi et al <img src="https://img.shields.io/badge/MICRO-2022-green.svg" alt="13-pages" align="top">
+ [QuCloud: A New Qubit Mapping Mechanism for Multi-programming Quantum Computing in Cloud Environment](https://ieeexplore.ieee.org/document/9407180) Lei Liu, Xinglei Dou <img src="https://img.shields.io/badge/HPCA-2021-green.svg" alt="13-pages" align="top">
+ [Optimal mapping for near-term quantum architectures based on Rydberg atoms](https://arxiv.org/abs/2109.04179) S.Brandhofer et al <img src="https://img.shields.io/badge/ICCAD-2021-green.svg" alt="13-pages" align="top">
+ [Time-optimal Qubit mapping](https://dl.acm.org/doi/pdf/10.1145/3445814.3446706) Chi Zhang et al <img src="https://img.shields.io/badge/ASPLOS-2021-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=_557jSReORo)

> Qubit Routing
+ [Quantum Routing with Teleportation](https://arxiv.org/pdf/2204.04185) Dhruv Devulapalli et al <img src="https://img.shields.io/badge/Physical Review Research-2024-green.svg" alt="13-pages" align="top">
+ [AlphaRouter: Quantum Circuit Routing with Reinforcement Learning and Tree Search](https://arxiv.org/pdf/2410.05115) Wei Tang et al <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="13-pages" align="top">
+ [Efficient Qubit Routing for a Globally Connected Trapped Ion Quantum Computer](https://arxiv.org/pdf/2002.12782) Mark Webber et al <img src="https://img.shields.io/badge/Advanced Quantum Technologies-2020-green.svg" alt="13-pages" align="top">
+ [On the Qubit Routing Problem](https://arxiv.org/pdf/1902.08091) Alexander Cowtan et al <img src="https://img.shields.io/badge/TQC-2019-green.svg" alt="13-pages" align="top">

> Circuit Scheduling 
+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) Toshinari Itoko, Takashi Imamichi <img src="https://img.shields.io/badge/QCE-2020-green.svg" alt="13-pages" align="top">
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) Gian Giacomo Guerreschi, Jongsoo Park <img src="https://img.shields.io/badge/Quantum Sci-2017-green.svg" alt="13-pages" align="top">

> Error-Aware & Noise-Aware Compilation

+ [Resource-Efficient Context-Aware Dynamical Decoupling Embedding for Arbitrary Large-Scale Quantum Algorithms](https://link.aps.org/doi/10.1103/PRXQuantum.6.010332) Paul Coote et al <img src="https://img.shields.io/badge/PRX Quantum-2025-green.svg" alt="13-pages" align="top">
+ [Learning high-accuracy error decoding for quantum processors](https://www.nature.com/articles/s41586-024-08148-8) Johannes Bausch et al <img src="https://img.shields.io/badge/Nature-2024-green.svg" alt="13-pages" align="top">
+ [Error Propagation-Aware Routing: A New Routing Strategy to Improve Success Rates of Quantum Circuits](https://dl.acm.org/doi/pdf/10.1145/3649476.3658790) Lu Fang et al <img src="https://img.shields.io/badge/ICCAD-2024-green.svg" alt="13-pages" align="top"> 
+ [Learning How to Dynamically Decouple](https://arxiv.org/html/2405.08689v1) Arefur Rahman et al <img src="https://img.shields.io/badge/Physical Review Applied-2024-green.svg" alt="13-pages" align="top">
+ [On the Use of Calibration Data in Error-Aware Compilation Techniques for NISQ Devices](https://arxiv.org/html/2407.21462v1) Handy Kurniawan et al <img src="https://img.shields.io/badge/2024-green.svg" alt="13-pages" align="top">
+ [VAQEM: A Variational Approach to Quantum Error Mitigation](https://www.computer.org/csdl/proceedings-article/hpca/2022/202700a288/1Ds0fvoYbCw) Gokul S. Ravi et al <img src="https://img.shields.io/badge/HPCA-2022-green.svg" alt="13-pages" align="top">
+ [ADAPT: Mitigating Idling Errors in Qubits via Adaptive Dynamical Decoupling](https://dl.acm.org/doi/10.1145/3466752.3480059) Poulami Das et al <img src="https://img.shields.io/badge/MICRO-2021-green.svg" alt="13-pages" align="top">
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503) Yongshan Ding et al <img src="https://img.shields.io/badge/MICRO-2020-green.svg" alt="13-pages" align="top">
+ [Digital Zero-Noise Extrapolation for Quantum Error Mitigation](https://arxiv.org/abs/2005.10921) Tudor Giurgica-Tiron et al <img src="https://img.shields.io/badge/QCE-2020-green.svg" alt="13-pages" align="top">
+ [A Noise-Aware Qubit Mapping Algorithm Evaluated via Qubit Interaction-Graph Criteria](https://www.researchgate.net/publication/350512755_A_Noise-Aware_Qubit_Mapping_Algorithm_Evaluated_via_Qubit_Interaction-Graph_Criteria) Matthew Steinberg et al <img src="https://img.shields.io/badge/QCS-2020-green.svg" alt="13-pages" align="top">
+ [Not All Qubits Are Created Equal: Variation-Aware Qubit Allocation in NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007) Swamit Tannu & Moinuddin Qureshi  <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" alt="13-pages" align="top">
+ [Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.](https://arxiv.org/abs/1901.11054) Prakash Murali et al <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" alt="13-pages" align="top"> [Youtube](https://youtu.be/4RlOaxYPkX8?si=CieyhIebX3hjo6rj)
+ [Practical Quantum Error Mitigation for Near-Future Applications](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509) Suguru Endo et al <img src="https://img.shields.io/badge/Physical Review X-2018-green.svg" alt="13-pages" align="top">
+ [Error Mitigation for Short-Depth Quantum Circuits](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509) Kristan Temme et al <img src="https://img.shields.io/badge/Physical Review Letter-2017-green.svg" alt="13-pages" align="top">

<h4 id="pulse-level-compile">Pulse-Level Compilation & Control</h4>

+ [A Synergistic Compilation Workflow for Tackling Crosstalk in Quantum Machines](https://arxiv.org/abs/2207.05751) Fei Hua et al <img src="https://img.shields.io/badge/Arxiv-2023-green.svg" alt="13-pages" align="top">
+ [Hybrid Gate-Pulse Model for Variational Quantum Algorithms](https://arxiv.org/abs/2212.00661) Zhiding Liang et al <img src="https://img.shields.io/badge/Arxiv-2022-green.svg" alt="13-pages" align="top">
+ [Enabling Pulse-Level Programming, Compilation, and Execution in XACC](https://arxiv.org/pdf/2003.11971) Thien Nguyen, Alexander McCaskey <img src="https://img.shields.io/badge/TC-2020-green.svg" alt="13-pages" align="top">
+ [Resource-Efficient Quantum Computing by Breaking Abstractions](https://arxiv.org/abs/2011.00028) Yunong Shi <img src="https://img.shields.io/badge/IEEE Journal-2020-green.svg" alt="13-pages" align="top">
+ [Optimized Quantum Compilation for Near-Term Algorithms with OpenPulse](https://arxiv.org/abs/2004.11205) Pranav Gokhale et al <img src="https://img.shields.io/badge/Arxiv-2020-green.svg" alt="13-pages" align="top"> [Youtube](https://youtu.be/dtPaDmE89Yc?si=5z1tfMK7FSw-SRsw)
+ [Software Mitigation of Crosstalk on Noisy Intermediate-Scale Quantum Computers](https://arxiv.org/pdf/2001.02826) Prakash Murali et al <img src="https://img.shields.io/badge/ASPLOS-2020-green.svg" alt="13-pages" align="top">
+ [Partial Compilation of Variational Algorithms for Near-term Quantum Machines](https://arxiv.org/pdf/1909.07522) Pranav Gokhale et al <img src="https://img.shields.io/badge/MICRO-2019-green.svg" alt="13-pages" align="top">

<h4 id="runtime-dynamic-execution">Runtime & Dynamic Execution</h4>

+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) Philipp Seitz et al <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/qc-tum/milq) 
+ [Qibolab: An Open-Source Hybrid Quantum Operating System](https://quantum-journal.org/papers/q-2024-02-12-1247/) Stavros Efthymiou et al <img src="https://img.shields.io/badge/Quantum Journal-2024-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/qiboteam/qibolab) 
+ [Combining Quantum Processors with Real-Time Classical Communication](https://www.nature.com/articles/s41586-024-08178-2) Almudena Carrera Vazquez et al <img src="https://img.shields.io/badge/Nature-2024-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/eggerdj/cut_graph_state_data) 

<h2 id="part-b-quantum-compiler-ecosystem">Part B: Quantum Compiler Ecosystem</h2>

<h4 id="quantum-testing-and-debugging">Quantum Testing and Debugging</h4>

+ [Testing and Debugging Quantum Programs: The Road to 2030](https://dl.acm.org/doi/10.1145/3715106) Neilson Carlos Leite Ramalho et al <img src="https://img.shields.io/badge/TOSEM-2025-green.svg" alt="13-pages" align="top">
+ [QuraTest: Automated Testing of Quantum Programs with Complex Input States](https://dl.acm.org/doi/10.1109/ASE56229.2023.00196) Jiaming Ye et al <img src="https://img.shields.io/badge/ASE-2023-green.svg" alt="13-pages" align="top">
+ [MorphQ: Metamorphic Testing for Quantum Programs](https://arxiv.org/abs/2206.01111) Matteo Paltenghi, Michael Pradel <img src="https://img.shields.io/badge/ICSE-2023-green.svg" alt="13-pages" align="top">
+ [QuCAT: Quantum Combinatorial Testing Framework](https://arxiv.org/abs/2309.00119) Xinying Wang et al <img src="https://img.shields.io/badge/ASE-2023-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=UsqgOudKLio)
+ [QuSBT: Search-Based Testing of Quantum Programs](https://dl.acm.org/doi/10.1145/3510454.3516839) Xinying Wang et al <img src="https://img.shields.io/badge/ICSE-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=Wh0FZ-kTglo)
+ [QMutPy: A Mutation Testing Tool for Quantum Algorithms and Applications in Qiskit](https://jose.github.io/assets/pdfs/ISSTA2022-tool-paper.pdf)  E. Fortunato et al <img src="https://img.shields.io/badge/ASE-2022-green.svg" alt="13-pages" align="top">
+ [Quito: A coverage-guided test generator for quantum programs](https://dl.acm.org/doi/abs/10.1109/ASE51524.2021.9678798) Xinyi Wang et al <img src="https://img.shields.io/badge/ASE -2021-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=kuI9QaCo8A8)
+ [Muskit: Mutation Testing for Qiskit Quantum Programs](https://ieeexplore.ieee.org/document/9678563) A. Mendiluze et al <img src="https://img.shields.io/badge/ASE-2021-green.svg" alt="13-pages" align="top">
+ [Projection-based runtime assertions for testing and debugging Quantum programs](https://dl.acm.org/doi/10.1145/3428218) Gushu Li et al <img src="https://img.shields.io/badge/OOPSLA-2020-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=7GVNWMR1NX4)
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/pdf/1810.00375) Thomas Häner et al <img src="https://img.shields.io/badge/OOPSLA-2020-green.svg" alt="13-pages" align="top">
+ [Statistical Assertions for Quantum Programs](https://arxiv.org/abs/1905.09721) Yipeng Huang, M. Martonosi <img src="https://img.shields.io/badge/ISCA-2019-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=Jic3OcJHmRg)

<h4 id="quantum-formal-verification">Quantum Formal Verification</h4>

+ [CoqQ: Foundational Verification of Quantum Programs](https://arxiv.org/abs/2207.11350) L. Zhou  <img src="https://img.shields.io/badge/POPL-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=RjKCP8U-1Zg)
+ [Twist: Sound Reasoning for Purity and Entanglement in Quantum Programs](https://arxiv.org/abs/2205.02287) Charles Yuan et al <img src="https://img.shields.io/badge/POPL-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=H3GIBgH5Ud4)
+ [Giallar: Push-Button Verification for the Qiskit Quantum Compiler](https://arxiv.org/pdf/2205.00661) Runzhou Tao at al <img src="https://img.shields.io/badge/PLDI-2022-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=m9pR53Zcj5w)
+ [Quantum Relational Hoare Logic](https://arxiv.org/abs/1802.03188) Dominique Unruh <img src="https://img.shields.io/badge/POPL-2019-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=U1-xP2SMDc0)
+ [QWIRE: A Core Language for Quantum Circuits](https://dl.acm.org/doi/10.1145/3009837.3009894) J. Paykin et al <img src="https://img.shields.io/badge/POPL-2017-green.svg" alt="13-pages" align="top">
+ [An Algebra of Quantum Processes](https://arxiv.org/abs/0707.0330) M. Ying et al <img src="https://img.shields.io/badge/TOCL-2019-green.svg" alt="13-pages" align="top">


<h4 id="lattice-surgery-surface-code-compilation">Lattice Surgery & Surface Code Compilation</h4>

+ [CaliQEC: In-situ Qubit Calibration for Surface Code Quantum Error Correction](https://dl.acm.org/doi/pdf/10.1145/3695053.3731042) <img src="https://img.shields.io/badge/ISCA-2025-green.svg" alt="13-pages" align="top"> 
+ [Dependency-Aware Compilation for Surface Code Quantum Architectures](https://arxiv.org/abs/2311.18042) Abtin Molavi et al <img src="https://img.shields.io/badge/OOPSLA-2025-green.svg" alt="13-pages" align="top">
+ [Lattice Surgery Compilation Beyond the Surface Code](https://arxiv.org/abs/2504.10591) Laura S. Herzog et al <img src="https://img.shields.io/badge/-2025-green.svg" alt="13-pages" align="top">
+ [A High Performance Compiler for Very Large Scale Surface Code Computations](https://arxiv.org/abs/2302.02459) George Watkins et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [A Resource-Allocating Compiler for Lattice Surgery](https://arxiv.org/abs/2506.04620) Alan Robertson et al <img src="https://img.shields.io/badge/QCS-2020-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/latticesurgery-com/lattice-surgery-compiler)
+ [Lattice Surgery Translation for Quantum Computation](https://arxiv.org/abs/1608.05208) Daniel Herr et al <img src="https://img.shields.io/badge/New Journal of Physics-2017-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/herr-d/LS_translation)
+ [Resource Optimized Quantum Architectures for Surface Code Implementations of Magic-State Distillation](https://arxiv.org/pdf/1904.11528) Adam Holmes et al




<h4 id="quantum-circuit-analysis">Quantum Circuit Analysis</h4>

+ [Character Complexity: A Novel Measure for Quantum Circuit Analysis](https://arxiv.org/abs/2408.09641) Daksh Shami <img src="https://img.shields.io/badge/2024-green.svg" alt="13-pages" align="top">
+ [QuCT: A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) Siwei Tan et al <img src="https://img.shields.io/badge/MICRO-2023-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/JanusQ/QuCT-Micro2023) 
+ [Quantum Vulnerability Analysis to Guide Robust Quantum Computing System Design](https://arxiv.org/pdf/2207.14446) Fang Qi et al <img src="https://img.shields.io/badge/TQE-2023-green.svg" alt="13-pages" align="top">
+ [Gleipnir: Toward Practical Error Analysis for Quantum Programs](https://arxiv.org/abs/2104.06349) Runzhou Tao et al <img src="https://img.shields.io/badge/PLDI-2021-green.svg" alt="13-pages" align="top">


<h4 id="quantum-compiler-emerging-topics">Emerging Topics</h4>

> Quantum Secure Compilation
+ [Obfuscation of Unitary Quantum Programs](https://arxiv.org/pdf/2507.11970) Mi-Ying Huang, Er-Cheng Tang <img src="https://img.shields.io/badge/2025-green.svg" alt="13-pages" align="top">
+ [OpaQue: Program Output Obfuscation for Quantum Software Circuits in Quantum Clouds](https://hpcrl.github.io/ICS2025-webpage/program/Proceedings_ICS25/ics25-32.pdf) Tirthak Patel et al <img src="https://img.shields.io/badge/ICS-2025-green.svg" alt="13-pages" align="top">
+ [TetrisLock: Quantum Circuit Split Compilation with Interlocking Patterns](https://arxiv.org/abs/2503.11982) Qian Wang et al <img src="https://img.shields.io/badge/DAC-2025-green.svg" alt="13-pages" align="top">  ￼
+ [OPAQUE: Obfuscating Phase in Quantum Circuit Compilation for Efficient IP Protection](https://www.arxiv.org/abs/2502.16605) Anees Rehman et al <img src="https://img.shields.io/badge/ISQED-2025-green.svg" alt="13-pages" align="top"> 
+ [Split Compilation for Security of Quantum Circuits](https://pure.psu.edu/en/publications/split-compilation-for-security-of-quantum-circuits) Abdullah Ash Saki et al <img src="https://img.shields.io/badge/ICCAD-2021-green.svg" alt="13-pages" align="top">
  
> Qudit Compilation
+ [MQT Qudits: A Software Framework for Mixed-Dimensional Quantum Computing](https://arxiv.org/abs/2410.02854) Lukas Burgholzer et al <img src="https://img.shields.io/badge/-2024-green.svg" alt="13-pages" align="top">
+ [Efficient, direct compilation of SU(N) operations into SNAP](https://arxiv.org/abs/2307.11900) Vladislav D. Kurpas et al <img src="https://img.shields.io/badge/Physical Review A-2023-green.svg" alt="13-pages" align="top">
+ [QudCom: Towards Quantum Compilation for Qudit Systems](https://arxiv.org/abs/2311.07015) Sebastian Brandhofer et al <img src="https://img.shields.io/badge/2023-green.svg" alt="13-pages" align="top">
+ [Compilation of Entangling Gates for High-Dimensional Quantum Processors](https://arxiv.org/abs/2301.04155) Manuel G. J. B. A. Cordier et al <img src="https://img.shields.io/badge/ASP DAC-2023-green.svg" alt="13-pages" align="top">
+ [Adaptive Compilation of Multi-Level Quantum Operations](https://arxiv.org/abs/2206.03842) David R. M. Arvidsson-Shukur et al <img src="https://img.shields.io/badge/QCE-2022-green.svg" alt="13-pages" align="top">

  
</br>

<h2 id="part-c-quantum-hardware-specific-compilation">Part C: Quantum Hardware Specific Compilation</h2>

<h4 id="superconducting-qc">Superconducting QC</h4>

+ [Selective Excitation of Superconducting Qubits with a Shared Control Line through Pulse Shaping](https://arxiv.org/pdf/2501.10710) Ryo Matsuda et al <img src="https://img.shields.io/badge/2025-green.svg" alt="13-pages" align="top">
+ [Virtual-Z Gates and Symmetric Gate Compilation](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.020348) Arian Vezvaee et al <img src="https://img.shields.io/badge/Physical Review X Quantum-2025-green.svg" alt="13-pages" align="top">
+ [CCMap: Hardware-Aware Compilation for Chip-to-Chip Coupler-Connected QPUs](https://arxiv.org/abs/2505.09036) Zefan Du et al <img src="https://img.shields.io/badge/2025-green.svg" alt="13-pages" align="top">
+ [Pulse-Based Variational Quantum Optimization and Metalearning in Superconducting Circuits](https://arxiv.org/abs/2407.12636) Yapeng Wang et al <img src="https://img.shields.io/badge/Arxiv-2024-green.svg" alt="13-pages" align="top">
+ [Direct Pulse-Level Compilation of Arbitrary Quantum Logic Gates on Superconducting Qutrits](https://arxiv.org/abs/2303.04261) Yujin Cho et al <img src="https://img.shields.io/badge/Physical Review Applied-2024-green.svg" alt="13-pages" align="top">
+ [Sensitivity-Adapted Closed-Loop Optimization for High-Fidelity CZ Gates](https://arxiv.org/abs/2412.17454) Niklas J. Glaser et al <img src="https://img.shields.io/badge/2024-green.svg" alt="13-pages" align="top">
+ [Implementing Fast and High-Fidelity Quantum Operations Using Open-Loop Optimal Control](https://arxiv.org/abs/2410.22603) LBNL Collaboration <img src="https://img.shields.io/badge/2024-green.svg" alt="13-pages" align="top">
+ [A Time Optimization Framework for Robust and Low-Latency Quantum Circuits](https://arxiv.org/abs/2412.18533) Eduardo W. Lussi et al <img src="https://img.shields.io/badge/Physical Review Applied-2024-green.svg" alt="13-pages" align="top">
+ [Optimized Compilation of Aggregated Instructions for Realistic Quantum Computers](https://arxiv.org/pdf/1902.01474) Yunong Shi et al <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" alt="13-pages" align="top">

<h4 id="trapped-ion-qc">Trapped-Ion QC</h4>

+ [Graph-Based Pulse Representation for Diverse Quantum Control Hardware](https://arxiv.org/abs/2409.08407) Aniket S. Dalvi et al <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="13-pages" align="top">
+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) Francesco Preti <img src="https://img.shields.io/badge/Quantum Journal-2024-green.svg" alt="13-pages" align="top">
+ [TISCC: A Surface Code Compiler and Resource Estimator for Trapped-Ion Processors](https://dl.acm.org/doi/abs/10.1145/3624062.3624214) Tyler Leblond et al <img src="https://img.shields.io/badge/SC-2023-green.svg" alt="13-pages" align="top">
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) Jonathan Durandau <img src="https://img.shields.io/badge/Quantum Journal-2023-green.svg" alt="13-pages" align="top"> [GitHub](https://github.com/cda-tum/mqt-ion-shuttler)  
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) Fabian Kreppel et al <img src="https://img.shields.io/badge/Quantum Journal-2022-green.svg" alt="13-pages" align="top">
+ [Backend compiler phases for trapped-ion quantum computers](https://arxiv.org/abs/2206.00544) T. Schmale et al <img src="https://img.shields.io/badge/QSW-2022-green.svg" alt="13-pages" align="top">
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) Xin-Chuan Wu <img src="https://img.shields.io/badge/HPCA-2020-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=SrcuokJUZp4)
  
<h4 id="neutral-atom-qc">Neutral-Atom QC</h4>

+ [Weaver: A Retargetable Compiler Framework for FPQA Quantum Architectures](https://arxiv.org/pdf/2409.07870) Oğuzcan Kırmemiş et al <img src="https://img.shields.io/badge/CGO-2025-green.svg" alt="13-pages" align="top">
+ [ConiQ: Enabling Concatenated Quantum Error Correction on Neutral Atom Arrays](https://arxiv.org/pdf/2508.05779) Pengyu Liu et al <img src="https://img.shields.io/badge/Arxiv-2025-green.svg" alt="13-pages" align="top">
+ [Atomique: A Quantum Compiler for Reconfigurable Neutral Atom Arrays](https://arxiv.org/pdf/2311.15123) Hanrui Wang et al <img src="https://img.shields.io/badge/ISCA-2024-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=uTsOfMIm23s)
+ [Pulse Family Optimization for Parametrized Quantum Gates Using Spectral Clustering](https://arxiv.org/abs/2408.00119) Robert de Keijzer et al <img src="https://img.shields.io/badge/Quantum Journal-2024-green.svg" alt="13-pages" align="top">
+ [Q-Pilot: Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) Hanrui Wang et al <img src="https://img.shields.io/badge/DAC-2024-green.svg" alt="13-pages" align="top">
+ [Compiling Quantum Circuits for Dynamically Field Programmable Neutral Atoms Array Processors](arxiv.org/pdf/2306.03487) Daniel Bochen Tan <img src="https://img.shields.io/badge/Quantum Journal-2024-green.svg" alt="13-pages" align="top">
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) S. Ebadi et al <img src="https://img.shields.io/badge/Science-2022-green.svg" alt="13-pages" align="top">
  
<h4 id="photonics-qc">Photonics QC</h4>

+ [OneAdapt: Adaptive Compilation for Resource-Constrained Photonic One-Way Quantum Computing](https://arxiv.org/abs/2504.17116) Hezi Zhang et al <img src="https://img.shields.io/badge/Micro-2025-green.svg" alt="13-pages" align="top">
+ [A Scalable and Robust Compilation Framework for Emitter-Photonic Quantum Computing](https://arxiv.org/abs/2503.16346) Xiangyu Ren et al <img src="https://img.shields.io/badge/DAC-2025-green.svg" alt="13-pages" align="top">
+ [OnePerc: A Randomness-aware Compiler for Photonic Quantum Computing](https://arxiv.org/abs/2403.01829) Hezi Zhang et al <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg" alt="13-pages" align="top"> [Youtube](https://www.youtube.com/watch?v=TLhNJRZUeas)
+ [OneQ: A Compilation Framework for Photonic One-Way Quantum Computation](https://arxiv.org/abs/2209.01545) Hezi Zhang et al <img src="https://img.shields.io/badge/ISCA-2023-green.svg" alt="13-pages" align="top">
+ [A Compiler for Universal Photonic Quantum Computers](https://arxiv.org/abs/2210.09251) Felix Zilk et al <img src="https://img.shields.io/badge/QCS-2022-green.svg" alt="13-pages" align="top">
+ [A Generic Measurement-Based Quantum Compilation Pipeline](https://arxiv.org/abs/2302.00795) Nader M. Mohammadizadeh et al <img src="https://img.shields.io/badge/Arxiv-2023-green.svg" alt="13-pages" align="top">
+ [Strawberry Fields: A Software Platform for Photonic Quantum Computing](https://arxiv.org/pdf/1804.03159) Nathan Killoran et al <img src="https://img.shields.io/badge/Quantum Journal-2018-green.svg" alt="13-pages" align="top">


<h4 id="silicon-spin-qubit-qc">Silicon Spin QC</h4>

+ [Compilation Techniques for Spin Qubits in a Shuttling Bus Architecture](https://arxiv.org/pdf/2502.06263) Pau Escofet et al <img src="https://img.shields.io/badge/ISCAS-2025-green.svg" alt="13-pages" align="top">
+ [Running a six-qubit quantum circuit on a silicon spin qubit array](https://arxiv.org/pdf/2505.19200) Fernández de Fuentes et al <img src="https://img.shields.io/badge/2025-green.svg" alt="13-pages" align="top">
+ [SpinQ: Compilation strategies for scalable spin-qubit architectures](https://arxiv.org/pdf/2301.13241) N. Paraskevopoulos et al <img src="https://img.shields.io/badge/TQC-2024-green.svg" alt="13-pages" align="top">
+ [Compilation and scaling strategies for a silicon quantum processor with sparse two-dimensional connectivity](https://arxiv.org/pdf/2201.02877) O. Crawford et al <img src="https://img.shields.io/badge/npj Quantum Information-2023-green.svg" alt="13-pages" align="top">

<h4 id="topological-qc">Topological QC (theoretical stage)</h4>

+ [Topological quantum compilation of metaplectic anyons based on the genetic optimized algorithms](https://arxiv.org/abs/2501.01745) Parsa Hosseini et al <img src="https://img.shields.io/badge/Physical Review Journals-2025-green.svg" alt="13-pages" align="top">
+ [Topological quantum compilation of two-qubit gates](https://arxiv.org/abs/2408.07132) Parsa Hosseini et al <img src="https://img.shields.io/badge/Physical Review Journals-2024-green.svg" alt="13-pages" align="top">
+ [Optimized Topological Quantum Compilation of Three-Qubit Controlled Gates in the Fibonacci Anyon Model](https://arxiv.org/abs/2311.17645) Parsa Hosseini et al <img src="https://img.shields.io/badge/Physical Review Journals-2023-green.svg" alt="13-pages" align="top">
+ [Asymptotically Optimal Topological Quantum Compiling](https://arxiv.org/abs/1310.4150) — Michael Freedman et al <img src="https://img.shields.io/badge/Mathematical Physics Journal-2013-green.svg" alt="13-pages" align="top">
+ [Topological Quantum Compiling](https://arxiv.org/abs/quant-ph/0610111) L. Hormozi et al <img src="https://img.shields.io/badge/Physical Review B-2006-green.svg" alt="13-pages" align="top">

<h2 id="part-d-conference-and-journal">Part D: Conference and Journal</h2>

<h4 id="conference-deadline">Top-tier Conference Deadline</h4>

+ January - [ICCAD](https://www.iccad-conf.com/) [CCS](https://www.sigsac.org/ccs/CCS2026/)
+ March - [OOPSLA](https://2025.splashcon.org/track/OOPSLA) [TQC](https://tqc-conference.org/) [QCE](https://easychair.org/cfp/QCE25)
+ April - [QCE](https://qce.quantum.ieee.org/) [MICRO](https://www.microarch.org/)
+ July - [POPL](https://conf.researchr.org/home/POPL-2026)
+ August - [ASPLOS](https://www.asplos-conference.org/) <summer cycle>
+ September - [HPCA](https://hpca-conf.org/) [QIP](https://qipconference.org/)
+ November - [CC](https://conf.researchr.org/series/cc) [ISCA](https://iscaconf.org/) [PLDI](https://conf.researchr.org/series/pldi) [DAC](https://www.dac.com/) [CGO](https://2026.cgo.org/) [STOC](https://acm-stoc.org/) [ICSE](https://conf.researchr.org/home/icse-2026)
 
<h4 id="journals">Journals</h4>

Impact Factor > 10
+ [Nature](https://www.nature.com/)
+ [Science](https://www.science.org/journal/science)
+ [Nature Machine Intelligence](https://www.nature.com/natmachintell/)
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

  



## Awesome Quantum Compiler 

By studying [Quantum Compilation](https://arxiv.org/abs/2112.00187) written by Marco Maronese (2021) and [Quantum Compilation Process](https://link.springer.com/chapter/10.1007/978-3-031-90200-0_9) by Javier Cardama et al. (2025), we can get a clear sense of how to enter and navigate the field of quantum compilation. I hope this collection supports your work as much as it supports mine. 🙂[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)


### Table of Contents
- [Fundamental and Survey Papers](#fundamental-and-survey)
- [NISQ Compilation](#nisq-compilation)
  - [Language, Assembly and IR Design](#language-assembly-ir)
  - [HW-agnostic Circuit Compilation](#hw-agnostic-compilation)
  - [Qubit Mapping and Routing](#qubit-mapping-and-routing)
  - [HW-aware Compilation](#hw-aware-compilation)
  - [Quantum Error Mitigation](#quantum-error-mitigation)
  - [Pulse-Level Compilation](#pulse-level-compile)
- [Fault-Tolerant Compilation](#fault-tolerant-compilation)
  - [QEC-Aware Compilation](#error-correction)
  - [Code-Specific Techniques](#code-specific-techniques)
  - [Magic State Distillation and Preparation](#magic-state-distillation-and-preparation)
  - [Distributed Quantum Compilation](#distributed-quantum-compilation)
 - [Quantum Compiler Ecosystem](#quantum-compiler-ecosystem)
  - [Quantum Testing and Debugging](#quantum-testing-and-debugging)
  - [Quantum Formal Verification](#quantum-formal-verification)  
  - [Quantum Secure Compilation](#quantum-secure-compilation)
- [Conference and Journal](#conference-and-journal) 

<h3 id="fundamental-and-survey">Fundamental and Survey Papers</h3>

+ <img src="https://img.shields.io/badge/ Bible -steelblue.svg" alt="17-pages" align="top"> [Quantum Computation and Quantum Information](https://profmcruz.wordpress.com/wp-content/uploads/2017/08/quantum-computation-and-quantum-information-nielsen-chuang.pdf) Michael Nielsen and Isaac Chuang
+ [Two-bit gates are universal for quantum computation](https://arxiv.org/abs/cond-mat/9407022) D. P. DiVincenzo <img src="https://img.shields.io/badge/Citations-1000+-blue.svg" alt="Citations: 1000" align="top"> (1994)
+ [Elementary gates for quantum computation](https://arxiv.org/abs/quant-ph/9503016) A. Barenco et al. <img src="https://img.shields.io/badge/Citations-4500+-blue.svg" alt="Citations: 3700" align="top"> (1995)
+ [Nonlocal properties of two-qubit gates and mixed states and optimization of quantum computations](https://arxiv.org/abs/quant-ph/0002045) Yuriy Makhlin (2000)
+ [Optimal Quantum Circuits for General Two-Qubit Gates](https://arxiv.org/abs/quant-ph/0308006) Farrokh Vatan, Colin Williams <img src="https://img.shields.io/badge/Citations-580+-blue.svg" alt="Citations: 300" align="top"> (2003)
+ [Improved simulation of stabilizer circuits](https://arxiv.org/abs/quant-ph/0406196) Scott Aaronson, Daniel Gottesman <img src="https://img.shields.io/badge/Citations-2100+-blue.svg" alt="Citations: 300" align="top"> (2004)
+ [Synthesis of quantum-logic circuits](https://arxiv.org/abs/quant-ph/0406176) Vivek V. Shende et al. <img src="https://img.shields.io/badge/Citations-1000+-blue.svg" alt="Citations: 300" align="top"> (2004)
+ [An Introduction to Cartan’s KAK Decomposition for QC Programmers](https://arxiv.org/abs/quant-ph/0507171) Robert R. Tucci <img src="https://img.shields.io/badge/Citations-580+-blue.svg" alt="Citations: 120+" align="top"> (2005)
+ [The Solovay-Kitaev algorithm](https://arxiv.org/abs/quant-ph/0505030) Christopher M. Dawson, Michael A. Nielsen <img src="https://img.shields.io/badge/Citations-900+-blue.svg" alt="Citations: 300" align="top"> (2005)
+ <img src="https://img.shields.io/badge/Survey paper-lightyellow.svg" alt="15-pages" align="top"> [Quantum Compiler Design for Qubit Mapping and Routing](https://arxiv.org/pdf/2505.16891) Chenghong zhu et al (2025)
+ <img src="https://img.shields.io/badge/Survey paper-lightyellow.svg" alt="15-pages" align="top"> [A Comprehensive Review of Quantum Circuit Optimization](https://www.mdpi.com/2624-960X/7/1/2) Krishnageetha Karuppasamy et al (2025)
+ <img src="https://img.shields.io/badge/Survey paper-lightyellow.svg" alt="15-pages" align="top"> [Quantum Circuit Synthesis and Compilation Optimization](https://arxiv.org/html/2407.00736v1) Ge Yan et al (2024)  
+ <img src="https://img.shields.io/badge/Google Quantum AI-slategray.svg" alt="15-pages" align="top"> [Quantum error correction below the surface code threshold](https://www.nature.com/articles/s41586-024-08449-y) (2025)
+ <img src="https://img.shields.io/badge/IBM Quantum-slategray.svg" alt="15-pages" align="top"> [High-threshold and low-overhead fault-tolerant quantum memory](https://www.nature.com/articles/s41586-025-08737-1) (2024)
+ <img src="https://img.shields.io/badge/PsiQuantum-slategray.svg" alt="15-pages" align="top"> [Fusion-based quantum computation](https://www.nature.com/articles/s41467-023-36493-1) (2023). [A manufacturable platform for photonic quantum computing](https://www.nature.com/articles/s41586-025-08820-7) (2025)
+ <img src="https://img.shields.io/badge/Quantinuum-slategray.svg" alt="15-pages" align="top"> [High-fidelity parallel entangling gates on a neutral-atom quantum computer](https://www.nature.com/articles/s41586-023-06481-y) (2023)
  
<h3 id="nisq-compilation">NISQ Compilation</h3>

<h4 id="language-assembly-ir">Language, Assembly and IR Design</h4>

+ [PHOENIX: Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) Zhaohui Yang et al <img src="https://img.shields.io/badge/DAC-2025-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/iqubit-org/phoenix)
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) Ali JavadiAbhari et al <img src="https://img.shields.io/badge/Parallel Comput-2022-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/epiqc/ScaffCC)
+ [PennyLane: Automatic differentiation of hybrid quantum-classical computations](https://arxiv.org/abs/1811.04968) Ville Bergholm et al [[Github]](https://github.com/PennyLaneAI/pennylane)
+ [STAQ: A Full-Stack Quantum Processing Toolkit](https://arxiv.org/abs/1912.06070) Matthew Amy, Vlad Gheorghiu  [[Github]](https://github.com/softwareQinc/staq)
+ [Programming languages and compiler design for realistic quantum hardware](https://www.nature.com/articles/nature23459) Frederic T. Chong <img src="https://img.shields.io/badge/Nature-2017-green.svg" alt="13-pages" align="top">
+ [ProjectQ: An Open Source Software Framework for Quantum Computing](https://arxiv.org/abs/1612.08091) Damian S. Steiger et al.  [[Github]](https://github.com/ProjectQ-Framework/ProjectQ)
+ [Design and architecture of the IBM Quantum Engine Compiler](https://arxiv.org/abs/2408.06469) Michael B. Healy et al. (2024)
+ [OpenQASM 3: A Broader and Deeper Quantum Assembly Language](https://arxiv.org/abs/2104.14722) Andrew W. Cross et al. (2021) [[Github]](https://github.com/openqasm/openqasm)
+ [Open Quantum Assembly Language](https://arxiv.org/abs/1707.03429) Andrew W. Cross et al. (2017)
+ [QASMTrans: A QASM based Quantum Transpiler Framework for NISQ Devices](https://arxiv.org/abs/2308.07581) Fei Hua et al <img src="https://img.shields.io/badge/SC-2023-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/pnnl/qasmtrans)
+ [ScaffCC: Scalable Compilation and Analysis of Quantum Programs](https://arxiv.org/abs/1507.01902) Ali JavadiAbhari et al
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) Anurudh Peduri, Siddharth Bhat <img src="https://img.shields.io/badge/CC-2022-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/opencompl/QMLIR)  
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) David Ittah et al <img src="https://img.shields.io/badge/TQC-2022-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/dime10/QIRO)
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) Alexander McCaskey, Thien Nguyen <img src="https://img.shields.io/badge/QCE-2021-green.svg" alt="13-pages" align="top">
+ [Quantum Circuit Transformations with a Multi-Level Intermediate Representation Compiler](https://arxiv.org/abs/2112.10677) Thien Nguyen et al <img src="https://img.shields.io/badge/arxiv-2021-green.svg" alt="13-pages" align="top"> 



<h4 id="hw-agnostic-compilation">HW-agnostic Circuit Compilation</h4>

+ [SuperstaQ: Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) Campbell et al. <img src="https://img.shields.io/badge/QCE-2023-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/Infleqtion/client-superstaq)
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/2109.03371) Gushu Li et al. <img src="https://img.shields.io/badge/ASPLOS-2022-green.svg" alt="13-pages" align="top"> [[Youtube]](https://youtu.be/lXFVkBlh9_Q?si=y_d4SgUwWQPwerch)
+ [A software methodology for compiling quantum programs](https://arxiv.org/abs/1604.01401) Thomas Häner et al <img src="https://img.shields.io/badge/Quantum Sci-2016-green.svg" alt="13-pages" align="top">
+ [Repeat-until-Success: Non-Deterministic Decomposition of Single-Qubit Unitaries](https://arxiv.org/abs/1311.1074) Adam Paetznick, Krysta Svore <img src="https://img.shields.io/badge/Quantum Information & Computation-2014-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/microsoft/Quantum/tree/main/samples/algorithms/repeat-until-success)
+ [Optimizing Quantum Circuits, Fast and Slow](https://arxiv.org/pdf/2411.04104) Amanda Xu et al <img src="https://img.shields.io/badge/ASPLOS-2025-green.svg" alt="13-pages" align="top">
+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) Francisco J. R. Ruiz <img src="https://img.shields.io/badge/Nature Machine Intelligence-2025-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/google-deepmind/alphatensor_quantum)
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) Zikun Li et al <img src="https://img.shields.io/badge/OOPSLA-2024-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/quantum-compiler/Quarl) [[Youtube]](https://youtu.be/DZjz88yDKC4?si=UTgp_1pQznhfs2Zs)
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) Bodo Rosenhahn, Tobias J. Osborne <img src="https://img.shields.io/badge/Physical Review Journal-2023-green.svg" alt="13-pages" align="top">
+ [Phase Gadget Synthesis for Shallow Circuit](https://arxiv.org/abs/1906.01734) Alexander Cowtan <img src="https://img.shields.io/badge/tket-PauliSquash(), OptimisePhaseGadgets()-yellow.svg" alt="Citations: 3700" align="top">
+ [Exact and Practical Pattern Matching for Quantum Circuit Optimization](https://arxiv.org/abs/1909.05270) Raban Iten et al <img src="https://img.shields.io/badge/Qiskit-TemplateOptimization()-yellow.svg" alt="Citations: 3700" align="top">
+ [Optimizing Clifford Circuits with Quantomatic](https://arxiv.org/abs/1901.10114) Andrew Fagan, Ross Duncan <img src="https://img.shields.io/badge/Qiskit-OptimizeCliffordT()-yellow.svg" alt="Citations: 3700" align="top">
+ [Automated optimization of large quantum circuits with continuous parameters](https://arxiv.org/abs/1710.07345) Yunseong Nam et al <img src="https://img.shields.io/badge/npj Quantum Information-2017-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/njross/optimizer)


> Qubit Allocation

+ [Machine-Learning-Based Qubit Allocation for Error Reduction in Quantum Circuits](https://ieeexplore.ieee.org/document/10209261) Travis LeCompte et al <img src="https://img.shields.io/badge/TQE-2023-green.svg" alt="13-pages" align="top">
+ [Qubit Allocation for Distributed Quantum Computing](https://ieeexplore.ieee.org/document/10228915) Yingling Mao et al <img src="https://img.shields.io/badge/INFOCOM-2023-green.svg" alt="13-pages" align="top">
+ [Qubit Allocation](https://hal.science/hal-01655951/file/Siraichi_QubitAllocation_CGO18.pdf) Marcos Siraichi et al <img src="https://img.shields.io/badge/CGO-2018-green.svg" alt="13-pages" align="top">


<h4 id="qubit-mapping-and-routing">Qubit Mapping and Routing</h4>

+ [S-SYNC: Shuttle & SWAP Co-Optimisation in QCCD](https://arxiv.org/abs/2505.01316) Chenghong Zhu et al <img src="https://img.shields.io/badge/ISCA-2025-green.svg" alt="13-pages" align="top">
+ [Compiling quantum circuits for dynamically field-programmable neutral atoms array processors](https://arxiv.org/pdf/2306.03487.pdf) Bochen Tan et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [Quantum Circuit Mapping Based on Incremental and Parallel SAT Solving](https://www.cs.cmu.edu/~mheule/publications/SATmap.pdf) Jiong Yang et al <img src="https://img.shields.io/badge/SAT-2024-green.svg" alt="13-pages" align="top">
+ [Fermihedral: On the Optimal Compilation for Fermion-to-Qubit Encoding](https://arxiv.org/pdf/2403.17794) Yuhao Liu et al <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=TLhNJRZUeas)
+ [Qubit mapping for reconfigurable atom arrays](https://dl.acm.org/doi/abs/10.1145/3508352.3549331) Bochen Tan et al <img src="https://img.shields.io/badge/ICCAD-2022-green.svg" alt="13-pages" align="top"> [[Youtube]](https://youtu.be/-tr8KtDKKDU?si=l2SwrXNY3KWvLOPz)
+ [Qubit Mapping and Routing via MaxSAT](https://arxiv.org/abs/2208.13679v1) Abtin Molavi et al <img src="https://img.shields.io/badge/MICRO-2022-green.svg" alt="13-pages" align="top">
+ [QuCloud: A New Qubit Mapping Mechanism for Multi-programming Quantum Computing in Cloud Environment](https://ieeexplore.ieee.org/document/9407180) Lei Liu, Xinglei Dou <img src="https://img.shields.io/badge/HPCA-2021-green.svg" alt="13-pages" align="top">
+ [Optimal mapping for near-term quantum architectures based on Rydberg atoms](https://arxiv.org/abs/2109.04179) S.Brandhofer et al <img src="https://img.shields.io/badge/ICCAD-2021-green.svg" alt="13-pages" align="top">
+ [Time-optimal Qubit mapping](https://dl.acm.org/doi/pdf/10.1145/3445814.3446706) Chi Zhang et al <img src="https://img.shields.io/badge/ASPLOS-2021-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=_557jSReORo)
+ [VF2++ An Improved Subgraph Isomorphism Algorithm](https://egres.elte.hu/tr/egres-18-03.pdf) Alpar J¨uttner and Peter Madarasi <img src="https://img.shields.io/badge/Qiskit-VF2Layout()-yellow.svg" alt="Citations: 3700" align="top">
+ [Quantum Routing with Teleportation](https://arxiv.org/pdf/2204.04185) Dhruv Devulapalli et al <img src="https://img.shields.io/badge/Physical Review Research-2024-green.svg" alt="13-pages" align="top">
+ [AlphaRouter: Quantum Circuit Routing with Reinforcement Learning and Tree Search](https://arxiv.org/pdf/2410.05115) Wei Tang et al <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="13-pages" align="top">
+ [Decomposing and Routing Quantum Circuits Under Constraints for Neutral Atom Architectures](https://arxiv.org/pdf/2307.14996) Natalia Nottingham et al <img src="https://img.shields.io/badge/Cirq-RouteCQC(), RoutingSwapTag()-yellow.svg" alt="Citations: 3700" align="top">
+ [2QAN: A quantum compiler for 2-local qubit Hamiltonian simulation algorithms](arxiv.org/pdf/2108.02099) Lingling Lao, Dan E. Browne <img src="https://img.shields.io/badge/ISCA-2022-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/lllingoo/2QAN) [[Youtube]](https://www.youtube.com/watch?v=rBThLSpNpVU) 
+ [Efficient Qubit Routing for a Globally Connected Trapped Ion Quantum Computer](https://arxiv.org/pdf/2002.12782) Mark Webber et al <img src="https://img.shields.io/badge/Advanced Quantum Technologies-2020-green.svg" alt="13-pages" align="top">
+ [Tackling the Qubit Mapping Problem for NISQ-Era Quantum Devices](https://arxiv.org/abs/1809.02573) Gushu Li et al <img src="https://img.shields.io/badge/Qiskit-SabreSwap()-yellow.svg" alt="Citations: 3700" align="top"> <img src="https://img.shields.io/badge/Qiskit-CheckMap()-yellow.svg" alt="Citations: 3700" align="top"> 
+ [On the Qubit Routing Problem](https://arxiv.org/pdf/1902.08091) Alexander Cowtan et al <img src="https://img.shields.io/badge/TQC-2019-green.svg" alt="13-pages" align="top"> <img src="https://img.shields.io/badge/tket-RoutingPass()-yellow.svg" alt="Citations: 3700" align="top">


> Qubit Scheduling

+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) Toshinari Itoko, Takashi Imamichi <img src="https://img.shields.io/badge/QCE-2020-green.svg" alt="13-pages" align="top">
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) Gian Giacomo Guerreschi, Jongsoo Park <img src="https://img.shields.io/badge/Quantum Sci-2017-green.svg" alt="13-pages" align="top">

<h4 id="hw-aware-compilation">HW-aware Compilation</h4>

> Superconducting

+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [Strong coupling of a single photon to a superconducting qubit using circuit quantum electrodynamics](https://www.nature.com/articles/nature02851) A.Wallraff et al (Nature, 2004) <img src="https://img.shields.io/badge/Citations-5000+-blue.svg" alt="Citations: 2500" align="top">
+ [Selective Excitation of Superconducting Qubits with a Shared Control Line through Pulse Shaping](https://arxiv.org/pdf/2501.10710) Ryo Matsuda et al <img src="https://img.shields.io/badge/arxiv-2025-green.svg" alt="13-pages" align="top">
+ [Virtual-Z Gates and Symmetric Gate Compilation](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.020348) Arian Vezvaee et al <img src="https://img.shields.io/badge/Physical Review X Quantum-2025-green.svg" alt="13-pages" align="top">
+ [CCMap: Hardware-Aware Compilation for Chip-to-Chip Coupler-Connected QPUs](https://arxiv.org/abs/2505.09036) Zefan Du et al <img src="https://img.shields.io/badge/arxiv-2025-green.svg" alt="13-pages" align="top">
+ [Bosehedral: Compiler Optimization for Bosonic Quantum Computing](https://arxiv.org/pdf/2402.02279) Junyu Zhou et al <img src="https://img.shields.io/badge/ISCA-2024-green.svg" alt="13-pages" align="top">
+ [Pulse-Based Variational Quantum Optimization and Metalearning in Superconducting Circuits](https://arxiv.org/abs/2407.12636) Yapeng Wang et al <img src="https://img.shields.io/badge/arxiv-2024-green.svg" alt="13-pages" align="top">
+ [Direct Pulse-Level Compilation of Arbitrary Quantum Logic Gates on Superconducting Qutrits](https://arxiv.org/abs/2303.04261) Yujin Cho et al <img src="https://img.shields.io/badge/Physical Review Applied-2024-green.svg" alt="13-pages" align="top">
+ [Sensitivity-Adapted Closed-Loop Optimization for High-Fidelity CZ Gates](https://arxiv.org/abs/2412.17454) Niklas J. Glaser et al <img src="https://img.shields.io/badge/arxiv-2024-green.svg" alt="13-pages" align="top">
+ [Implementing Fast and High-Fidelity Quantum Operations Using Open-Loop Optimal Control](https://arxiv.org/abs/2410.22603) LBNL Collaboration <img src="https://img.shields.io/badge/2024-green.svg" alt="13-pages" align="top">
+ [A Time Optimization Framework for Robust and Low-Latency Quantum Circuits](https://arxiv.org/abs/2412.18533) Eduardo W. Lussi et al <img src="https://img.shields.io/badge/Physical Review Applied-2024-green.svg" alt="13-pages" align="top">
+ [Optimized Compilation of Aggregated Instructions for Realistic Quantum Computers](https://arxiv.org/pdf/1902.01474) Yunong Shi et al <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" alt="13-pages" align="top">

> Trapped-Ion

+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [Quantum computations with cold trapped ions](https://www.fuw.edu.pl/~szczytko/NT/materialy/9_QC/Cirac_Zoller_PRL1995.pdf) J. I. Cirac and P. Zoller <img src="https://img.shields.io/badge/Citations-6200+-blue.svg" alt="Citations: 3500" align="top"> <img src="https://img.shields.io/badge/Qiskit-CheckGateDirection()-yellow.svg" alt="Citations: 3700" align="top">
+ [Graph-Based Pulse Representation for Diverse Quantum Control Hardware](https://arxiv.org/abs/2409.08407) Aniket S. Dalvi et al <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="13-pages" align="top">
+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) Francesco Preti <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [TISCC: A Surface Code Compiler and Resource Estimator for Trapped-Ion Processors](https://dl.acm.org/doi/abs/10.1145/3624062.3624214) Tyler Leblond et al <img src="https://img.shields.io/badge/SC-2023-green.svg" alt="13-pages" align="top">
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) Jonathan Durandau <img src="https://img.shields.io/badge/Quantum-2023-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/cda-tum/mqt-ion-shuttler)  
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) Fabian Kreppel et al <img src="https://img.shields.io/badge/Quantum-2022-green.svg" alt="13-pages" align="top">
+ [Backend compiler phases for trapped-ion quantum computers](https://arxiv.org/abs/2206.00544) T. Schmale et al <img src="https://img.shields.io/badge/QSW-2022-green.svg" alt="13-pages" align="top">
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) Xin-Chuan Wu <img src="https://img.shields.io/badge/HPCA-2020-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=SrcuokJUZp4)
  
> Neutral atom

+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [Rydberg Blockade & Neutral Atoms for Quantum Information](https://arxiv.org/abs/quant-ph/0108118) M. Saffman et al (APS Journal, 2010) <img src="https://img.shields.io/badge/Citations-3700+-blue.svg" alt="Citations: 2500" align="top">
+ [Weaver: A Retargetable Compiler Framework for FPQA Quantum Architectures](https://arxiv.org/pdf/2409.07870) Oğuzcan Kırmemiş et al <img src="https://img.shields.io/badge/CGO-2025-green.svg" alt="13-pages" align="top">
+ [ConiQ: Enabling Concatenated Quantum Error Correction on Neutral Atom Arrays](https://arxiv.org/pdf/2508.05779) Pengyu Liu et al <img src="https://img.shields.io/badge/arxiv-2025-green.svg" alt="13-pages" align="top">
+ [Atomique: A Quantum Compiler for Reconfigurable Neutral Atom Arrays](https://arxiv.org/pdf/2311.15123) Hanrui Wang et al <img src="https://img.shields.io/badge/ISCA-2024-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=uTsOfMIm23s)
+ [Pulse Family Optimization for Parametrized Quantum Gates Using Spectral Clustering](https://arxiv.org/abs/2408.00119) Robert de Keijzer et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [Q-Pilot: Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) Hanrui Wang et al <img src="https://img.shields.io/badge/DAC-2024-green.svg" alt="13-pages" align="top">
+ [Compiling Quantum Circuits for Dynamically Field Programmable Neutral Atoms Array Processors](arxiv.org/pdf/2306.03487) Daniel Bochen Tan <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) S. Ebadi et al <img src="https://img.shields.io/badge/Science-2022-green.svg" alt="13-pages" align="top">
  
> Photonics

+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [A scheme for efficient quantum computation with linear optics](https://arxiv.org/abs/quant-ph/0108118) E. Knill et al.(Nature, 2001) <img src="https://img.shields.io/badge/Citations-2500+-blue.svg" alt="Citations: 2500" align="top">
+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [A one-way quantum computer](https://arxiv.org/abs/quant-ph/0108118) R. Raussendorf and H. J. Briegel (Physical Review Letters, 2001) <img src="https://img.shields.io/badge/Citations-2500+-blue.svg" alt="Citations: 2500" align="top">
+ [OneAdapt: Adaptive Compilation for Resource-Constrained Photonic One-Way Quantum Computing](https://arxiv.org/abs/2504.17116) Hezi Zhang et al <img src="https://img.shields.io/badge/MICRO-2025-green.svg" alt="13-pages" align="top">
+ [A Scalable and Robust Compilation Framework for Emitter-Photonic Quantum Computing](https://arxiv.org/abs/2503.16346) Xiangyu Ren et al <img src="https://img.shields.io/badge/DAC-2025-green.svg" alt="13-pages" align="top">
+ [OnePerc: A Randomness-aware Compiler for Photonic Quantum Computing](https://arxiv.org/abs/2403.01829) Hezi Zhang et al <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=TLhNJRZUeas)
+ [OneQ: A Compilation Framework for Photonic One-Way Quantum Computation](https://arxiv.org/abs/2209.01545) Hezi Zhang et al <img src="https://img.shields.io/badge/ISCA-2023-green.svg" alt="13-pages" align="top">
+ [A Compiler for Universal Photonic Quantum Computers](https://arxiv.org/abs/2210.09251) Felix Zilk et al <img src="https://img.shields.io/badge/QCS-2022-green.svg" alt="13-pages" align="top">
+ [A Generic Measurement-Based Quantum Compilation Pipeline](https://arxiv.org/abs/2302.00795) Nader M. Mohammadizadeh et al <img src="https://img.shields.io/badge/2023-green.svg" alt="13-pages" align="top">
+ [Strawberry Fields: A Software Platform for Photonic Quantum Computing](https://arxiv.org/pdf/1804.03159) Nathan Killoran et al <img src="https://img.shields.io/badge/Quantum-2018-green.svg" alt="13-pages" align="top">

 
<h4 id="quantum-error-mitigation">Quantum Error Mitigation</h4>

+ [VAQEM: A Variational Approach to Quantum Error Mitigation](https://www.computer.org/csdl/proceedings-article/hpca/2022/202700a288/1Ds0fvoYbCw) Gokul S. Ravi et al <img src="https://img.shields.io/badge/HPCA-2022-green.svg" alt="13-pages" align="top">
+ [ADAPT: Mitigating Idling Errors in Qubits via Adaptive Dynamical Decoupling](https://dl.acm.org/doi/10.1145/3466752.3480059) Poulami Das et al <img src="https://img.shields.io/badge/MICRO-2021-green.svg" alt="13-pages" align="top">
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503) Yongshan Ding et al <img src="https://img.shields.io/badge/MICRO-2020-green.svg" alt="13-pages" align="top">
+ [Digital Zero-Noise Extrapolation for Quantum Error Mitigation](https://arxiv.org/abs/2005.10921) Tudor Giurgica-Tiron et al <img src="https://img.shields.io/badge/QCE-2020-green.svg" alt="13-pages" align="top">
+ [Practical Quantum Error Mitigation for Near-Future Applications](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509) Suguru Endo et al <img src="https://img.shields.io/badge/Physical Review X-2018-green.svg" alt="13-pages" align="top">
+ [Error Mitigation for Short-Depth Quantum Circuits](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509) Kristan Temme et al <img src="https://img.shields.io/badge/Physical Review Letter-2017-green.svg" alt="13-pages" align="top">

<h4 id="pulse-level-compile">Pulse-Level Compilation</h4>

+ [Towards a pulse-level intermediate representation for diverse quantum control systems](https://arxiv.org/abs/2507.15995) Jude Alnas et al. <img src="https://img.shields.io/badge/2025-green.svg" alt="13-pages" align="top"> 
+ [Enhancing Noisy Quantum Sensing by GHZ State Partitioning](https://arxiv.org/pdf/2507.02829) Allen Zang et al. <img src="https://img.shields.io/badge/QCE-2025-green.svg" alt="13-pages" align="top">
+ [Graph-Based Pulse Representation for Diverse Quantum Control Hardware](https://arxiv.org/abs/2409.08407) Aniket S. Dalvi et al. <img src="https://img.shields.io/badge/Computer Society-2024-green.svg" alt="13-pages" align="top">
+ [Variational Quantum Pulse Learning](https://arxiv.org/abs/2203.17267) Zhiding Liang et al. <img src="https://img.shields.io/badge/QCE-2022-green.svg" alt="13-pages" align="top">
+ [Enabling Pulse-Level Programming, Compilation, and Execution in XACC](https://arxiv.org/pdf/2003.11971) Thien Nguyen, Alexander McCaskey <img src="https://img.shields.io/badge/TC-2020-green.svg" alt="13-pages" align="top">
+ [Resource-Efficient Quantum Computing by Breaking Abstractions](https://arxiv.org/abs/2011.00028) Yunong Shi <img src="https://img.shields.io/badge/IEEE-2020-green.svg" alt="13-pages" align="top">
+ [Optimized Quantum Compilation for Near-Term Algorithms with OpenPulse](https://arxiv.org/abs/2004.11205) Pranav Gokhale et al <img src="https://img.shields.io/badge/Arxiv-2020-green.svg" alt="13-pages" align="top"> [[Youtube]](https://youtu.be/dtPaDmE89Yc?si=5z1tfMK7FSw-SRsw)
+ [Software Mitigation of Crosstalk on Noisy Intermediate-Scale Quantum Computers](https://arxiv.org/pdf/2001.02826) Prakash Murali et al <img src="https://img.shields.io/badge/ASPLOS-2020-green.svg" alt="13-pages" align="top"> <img src="https://img.shields.io/badge/Qiskit-CrosstalkAdaptiveLayout()-yellow.svg" alt="Citations: 3700" align="top">
+ [Partial Compilation of Variational Algorithms for Near-term Quantum Machines](https://arxiv.org/pdf/1909.07522) Pranav Gokhale et al <img src="https://img.shields.io/badge/MICRO-2019-green.svg" alt="13-pages" align="top">

<h3 id="quantum-compiler-ecosystem">Quantum Compiler Ecosystem</h3>

<h4 id="quantum-testing-and-debugging">Quantum Testing and Debugging</h4>

+ [Testing and Debugging Quantum Programs: The Road to 2030](https://dl.acm.org/doi/10.1145/3715106) Neilson Carlos Leite Ramalho et al <img src="https://img.shields.io/badge/TOSEM-2025-green.svg" alt="13-pages" align="top">
+ [QuraTest: Automated Testing of Quantum Programs with Complex Input States](https://dl.acm.org/doi/10.1109/ASE56229.2023.00196) Jiaming Ye et al <img src="https://img.shields.io/badge/ASE-2023-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/ToolmanInside/quratest-mutators)
+ [MorphQ: Metamorphic Testing for Quantum Programs](https://arxiv.org/abs/2206.01111) Matteo Paltenghi, Michael Pradel <img src="https://img.shields.io/badge/ICSE-2023-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/sola-st/MorphQ-Quantum-Qiskit-Testing-ICSE-23)
+ [QuCAT: Quantum Combinatorial Testing Framework](https://arxiv.org/abs/2309.00119) Xinying Wang et al <img src="https://img.shields.io/badge/ASE-2023-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=UsqgOudKLio)
+ [QuSBT: Search-Based Testing of Quantum Programs](https://dl.acm.org/doi/10.1145/3510454.3516839) Xinying Wang et al <img src="https://img.shields.io/badge/ICSE-2022-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=Wh0FZ-kTglo)
+ [QMutPy: A Mutation Testing Tool for Quantum Algorithms and Applications in Qiskit](https://jose.github.io/assets/pdfs/ISSTA2022-tool-paper.pdf)  E. Fortunato et al <img src="https://img.shields.io/badge/ASE-2022-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/jose/qmutpy-experiments)
+ [Quito: A coverage-guided test generator for quantum programs](https://dl.acm.org/doi/abs/10.1109/ASE51524.2021.9678798) Xinyi Wang et al <img src="https://img.shields.io/badge/ASE -2021-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/Simula-COMPLEX/quito) [[Youtube]](https://www.youtube.com/watch?v=kuI9QaCo8A8) 
+ [Muskit: Mutation Testing for Qiskit Quantum Programs](https://ieeexplore.ieee.org/document/9678563) A. Mendiluze et al <img src="https://img.shields.io/badge/ASE-2021-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/Simula-COMPLEX/muskit)
+ [Projection-based runtime assertions for testing and debugging Quantum programs](https://dl.acm.org/doi/10.1145/3428218) Gushu Li et al <img src="https://img.shields.io/badge/OOPSLA-2020-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=7GVNWMR1NX4)
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/pdf/1810.00375) Thomas Häner et al <img src="https://img.shields.io/badge/OOPSLA-2020-green.svg" alt="13-pages" align="top">
+ [Statistical Assertions for Quantum Programs](https://arxiv.org/abs/1905.09721) Yipeng Huang, M. Martonosi <img src="https://img.shields.io/badge/ISCA-2019-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=Jic3OcJHmRg)



<h4 id="quantum-formal-verification">Quantum Formal Verification</h4>

+ [Efficient Formal Verification of Quantum Error Correcting Programs](https://arxiv.org/abs/2504.07732) Qifan Huang et al. <img src="https://img.shields.io/badge/PLDI-2025-green.svg" alt="13-pages" align="top"> 
+ [QbC: Quantum Correctness by Construction](https://arxiv.org/abs/2307.15641) Anurudh Peduri et al. OOPSLA <img src="https://img.shields.io/badge/OOPSLA-2025-green.svg" alt="13-pages" align="top"> 
+ [Symbolic Execution for Quantum Error Correction Programs](https://arxiv.org/pdf/2311.11313) Wang Fang, Mingsheng Ying. PLDI <img src="https://img.shields.io/badge/PLDI-2024-green.svg" alt="13-pages" align="top"> 
+ [Quantum Probabilistic Model Checking for Time-Bounded Properties](https://dl.acm.org/doi/10.1145/3689731) Seungmin Jeon et al. <img src="https://img.shields.io/badge/OOPSLA-2024-green.svg" alt="13-pages" align="top"> 
+ [CoqQ: Foundational Verification of Quantum Programs](https://arxiv.org/abs/2207.11350) L. Zhou  <img src="https://img.shields.io/badge/POPL-2022-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=RjKCP8U-1Zg)
+ [Twist: Sound Reasoning for Purity and Entanglement in Quantum Programs](https://arxiv.org/abs/2205.02287) Charles Yuan et al <img src="https://img.shields.io/badge/POPL-2022-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=H3GIBgH5Ud4)
+ [Giallar: Push-Button Verification for the Qiskit Quantum Compiler](https://arxiv.org/pdf/2205.00661) Runzhou Tao at al <img src="https://img.shields.io/badge/PLDI-2022-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=m9pR53Zcj5w)
+ [Quantum Relational Hoare Logic](https://arxiv.org/abs/1802.03188) Dominique Unruh <img src="https://img.shields.io/badge/POPL-2019-green.svg" alt="13-pages" align="top"> [[Youtube]](https://www.youtube.com/watch?v=U1-xP2SMDc0)
+ [QWIRE: A Core Language for Quantum Circuits](https://dl.acm.org/doi/10.1145/3009837.3009894) J. Paykin et al <img src="https://img.shields.io/badge/POPL-2017-green.svg" alt="13-pages" align="top"> [[Github]](https://github.com/inQWIRE/QWIRE)
+ [Hoare Logic for Quantum Programs](https://arxiv.org/abs/0906.4586) Mingsheng Ying <img src="https://img.shields.io/badge/Qiskit-HoareOptimizer()-yellow.svg" alt="Citations: 3700" align="top">


<h4 id="quantum-secure-compilation">Quantum Secure Compilation</h4>

+ [Obfuscation of Unitary Quantum Programs](https://arxiv.org/pdf/2507.11970) Mi-Ying Huang, Er-Cheng Tang <img src="https://img.shields.io/badge/2025-green.svg" alt="13-pages" align="top">
+ [OpaQue: Program Output Obfuscation for Quantum Software Circuits in Quantum Clouds](https://hpcrl.github.io/ICS2025-webpage/program/Proceedings_ICS25/ics25-32.pdf) Tirthak Patel et al <img src="https://img.shields.io/badge/ICS-2025-green.svg" alt="13-pages" align="top">
+ [TetrisLock: Quantum Circuit Split Compilation with Interlocking Patterns](https://arxiv.org/abs/2503.11982) Qian Wang et al <img src="https://img.shields.io/badge/DAC-2025-green.svg" alt="13-pages" align="top">  ￼
+ [OPAQUE: Obfuscating Phase in Quantum Circuit Compilation for Efficient IP Protection](https://www.arxiv.org/abs/2502.16605) Anees Rehman et al <img src="https://img.shields.io/badge/ISQED-2025-green.svg" alt="13-pages" align="top"> 
+ [E-loq: Enhanced locking for quantum circuit IP protection](https://arxiv.org/abs/2412.17101) Y Liu et al <img src="https://img.shields.io/badge/QCE-2025-green.svg" alt="IP-Protection" align="top">
+ [Obfuscating quantum hybrid-classical algorithms for security and privacy](https://arxiv.org/abs/2305.02379) S Upadhyay, S Ghosh <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="Hybrid-Algo" align="top">
+ [Leveraging Quantum Circuit Cutting for Obfuscation and Intellectual Property Protection](https://arxiv.org/pdf/2511.04842) G Typaldos, W Tang, J Szefer <img src="https://img.shields.io/badge/QCE-2024-green.svg" alt="Circuit-Cutting" align="top">
+ [Split Compilation for Security of Quantum Circuits](https://pure.psu.edu/en/publications/split-compilation-for-security-of-quantum-circuits) Abdullah Ash Saki et al <img src="https://img.shields.io/badge/ICCAD-2021-green.svg" alt="13-pages" align="top">

</br>

> Ecosystem Niche Fields

+ <img src="https://img.shields.io/badge/Quantum OS-lightyellow.svg" alt="15-pages" align="top"> [An operating system for executing applications on quantum network nodes](https://www.nature.com/articles/s41586-025-08704-w) C. Delle Donne et al. <img src="https://img.shields.io/badge/Nature-2025-green.svg" alt="13-pages" align="top">
+ <img src="https://img.shields.io/badge/Quantum OS-lightyellow.svg" alt="15-pages" align="top"> [QOS: A Quantum Operating System](https://arxiv.org/abs/2406.19120) Emmanouil Giortamis et al. <img src="https://img.shields.io/badge/OSDI-2025-green.svg" alt="13-pages" align="top">
+ <img src="https://img.shields.io/badge/Quantum Firmware-lightyellow.svg" alt="15-pages" align="top"> [Towards Quantum-Resistant Trusted Computing](https://www.arxiv.org/abs/2601.11095) Grazia D'Onghia, Antonio Lioy. 2026
+ <img src="https://img.shields.io/badge/Control System-lightyellow.svg" alt="15-pages" align="top"> [A Generator for Real-Time Quantum Control System-on-Chips Compatible with RISC-V](https://arxiv.org/abs/2505.14902) Junyi Liu et al. 2025
+ <img src="https://img.shields.io/badge/Quantum Runtime-lightyellow.svg" alt="15-pages" align="top"> [Recent quantum runtime (dis)advantages](https://arxiv.org/abs/2510.06337) J. Tuziemski et al. 2025
+ <img src="https://img.shields.io/badge/Quantum Internet-lightyellow.svg" alt="15-pages" align="top"> [The Quantum Internet (Technical Version)](https://arxiv.org/abs/2501.12107) Peter P. Rohde et al. 2025
+ <img src="https://img.shields.io/badge/Architecture Search-lightyellow.svg" alt="15-pages" align="top"> [Quantum Architecture Search: A Survey](https://arxiv.org/abs/2406.06210) Darya Martyniuk et al. 2024
+ <img src="https://img.shields.io/badge/Circuit Analysis-lightyellow.svg" alt="15-pages" align="top"> [A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) Siwei Tan et al 
+ <img src="https://img.shields.io/badge/Circuit Analysis-lightyellow.svg" alt="15-pages" align="top"> [Gleipnir: Toward Practical Error Analysis for Quantum Programs](https://arxiv.org/abs/2104.06349) Runzhou Tao et al <img src="https://img.shields.io/badge/PLDI-2021-green.svg" alt="13-pages" align="top">


<h3 id="fault-tolerant-compilation">Fault-Tolerant Compilation</h3>

+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [Error correcting codes in quantum theory](https://users.physics.ox.ac.uk/~Steane/qec/Steane_PRL95.pdf) A. M. Steane (Physical Review Letters, 1996) <img src="https://img.shields.io/badge/Citations-3700+-blue.svg" alt="Citations: 2500" align="top">
+ <img src="https://img.shields.io/badge/Classic-lightblue.svg" alt="17-pages" align="top"> [Fault-tolerant quantum computation](https://arxiv.org/abs/quant-ph/9712048) J. Preskill (Proceedings of the Royal Society A, 1998) <img src="https://img.shields.io/badge/Citations-670-blue.svg" alt="Citations: 670" align="top">

<h4 id="error-correction">QEC-aware Compilation</h4>

+ [Resource-Efficient Context-Aware Dynamical Decoupling Embedding for Arbitrary Large-Scale Quantum Algorithms](https://link.aps.org/doi/10.1103/PRXQuantum.6.010332) Paul Coote et al <img src="https://img.shields.io/badge/PRX Quantum-2025-green.svg" alt="13-pages" align="top">
+ [Learning high-accuracy error decoding for quantum processors](https://www.nature.com/articles/s41586-024-08148-8) Johannes Bausch et al <img src="https://img.shields.io/badge/Nature-2024-green.svg" alt="13-pages" align="top">
+ [Error Propagation-Aware Routing: A New Routing Strategy to Improve Success Rates of Quantum Circuits](https://dl.acm.org/doi/pdf/10.1145/3649476.3658790) Lu Fang et al <img src="https://img.shields.io/badge/ICCAD-2024-green.svg" alt="13-pages" align="top"> 
+ [Learning How to Dynamically Decouple](https://arxiv.org/html/2405.08689v1) Arefur Rahman et al <img src="https://img.shields.io/badge/Physical Review Applied-2024-green.svg" alt="13-pages" align="top">
+ [On the Use of Calibration Data in Error-Aware Compilation Techniques for NISQ Devices](https://arxiv.org/html/2407.21462v1) Handy Kurniawan et al <img src="https://img.shields.io/badge/2024-green.svg" alt="13-pages" align="top">
+ [A Noise-Aware Qubit Mapping Algorithm Evaluated via Qubit Interaction-Graph Criteria](https://www.researchgate.net/publication/350512755_A_Noise-Aware_Qubit_Mapping_Algorithm_Evaluated_via_Qubit_Interaction-Graph_Criteria) Matthew Steinberg et al <img src="https://img.shields.io/badge/QCS-2020-green.svg" alt="13-pages" align="top">
+ [Not All Qubits Are Created Equal: Variation-Aware Qubit Allocation in NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007) Swamit Tannu & Moinuddin Qureshi  <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" alt="13-pages" align="top">
+ [Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.](https://arxiv.org/abs/1901.11054) Prakash Murali et al <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" alt="13-pages" align="top"> [[Youtube]](https://youtu.be/4RlOaxYPkX8?si=CieyhIebX3hjo6rj)

<h4 id="code-specific-techniques">Code-Specific Techniques</h4>

+ [CaliQEC: In-situ Qubit Calibration for Surface Code Quantum Error Correction](https://dl.acm.org/doi/pdf/10.1145/3695053.3731042) <img src="https://img.shields.io/badge/ISCA-2025-green.svg" alt="13-pages" align="top">
+ [A Resource-Allocating Compiler for Lattice Surgery](https://arxiv.org/abs/2506.04620) Alan Robertson et al <img src="https://img.shields.io/badge/QCS-2025-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/latticesurgery-com/lattice-surgery-compiler)
+ [Dependency-Aware Compilation for Surface Code Quantum Architectures](https://arxiv.org/abs/2311.18042) Abtin Molavi et al <img src="https://img.shields.io/badge/OOPSLA-2025-green.svg" alt="13-pages" align="top">
+ [Lattice Surgery Compilation Beyond the Surface Code](https://arxiv.org/abs/2504.10591) Laura S. Herzog et al <img src="https://img.shields.io/badge/-2025-green.svg" alt="13-pages" align="top">
+ [A High Performance Compiler for Very Large Scale Surface Code Computations](https://arxiv.org/abs/2302.02459) George Watkins et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg" alt="13-pages" align="top">
+ [Realistic Cost to Execute Practical Quantum Circuits using Direct Clifford+T Lattice Surgery Compilation](https://arxiv.org/abs/2311.10686) Tyler LeBlond et al <img src="https://img.shields.io/badge/TQC-2024-green.svg" alt="13-pages" align="top">
+ [Surface code compilation via edge-disjoint paths](https://arxiv.org/abs/2110.11493) Michael Beverland et al <img src="https://img.shields.io/badge/PRX Quantum-2022-green.svg" alt="13-pages" align="top">
+ [A Game of Surface Codes: Large-Scale Quantum Computing with Lattice Surgery](https://arxiv.org/abs/1808.02892) Daniel Litinski <img src="https://img.shields.io/badge/Quantum-2019-green.svg" alt="13-pages" align="top"> <img src="https://img.shields.io/badge/Qiskit-LitinskiTransformation()-yellow.svg" alt="Citations: 3700" align="top">
+ [Lattice Surgery Translation for Quantum Computation](https://arxiv.org/abs/1608.05208) Daniel Herr et al <img src="https://img.shields.io/badge/New Journal of Physics-2017-green.svg" alt="13-pages" align="top"> [[GitHub]](https://github.com/latticesurgery-com/lattice-surgery-compiler)
+ [Resource Optimized Quantum Architectures for Surface Code Implementations of Magic-State Distillation](https://arxiv.org/pdf/1904.11528) Adam Holmes et al

<h4 id="magic-state-distillation-and-preparation">Magic State Distillation and Preparation</h4>

+ [Orchestrating multi-level magic state distillation: a dynamic pipeline architecture](https://arxiv.org/abs/2509.24402) Junshi Wang and Prakash Murali <img src="https://img.shields.io/badge/arXiv-2025-green.svg" alt="paper" align="top">
+ [Locality-Aware Pauli-Based Computation for Local Magic State Preparation](https://arxiv.org/abs/2504.12091) Keita Kanno et al <img src="https://img.shields.io/badge/QCE-2025-green.svg" alt="paper" align="top">
+ [Realistic Cost to Execute Practical Quantum Circuits using Direct Clifford+T Lattice Surgery Compilation](https://arxiv.org/abs/2311.10686) Tyler Leblond et al <img src="https://img.shields.io/badge/TQC-2024-green.svg" alt="28-pages" align="top">
+ [Fault-tolerant, high-level quantum circuits: form, compilation and description](https://arxiv.org/abs/1509.02004) Alexandru Paler et al <img src="https://img.shields.io/badge/QST-2017-green.svg" alt="paper" align="top">
+ [Magic state distillation and gate compilation in quantum algorithms for quantum chemistry](https://arxiv.org/abs/1501.01298) Earl T. Campbell and J. O'Gorman <img src="https://img.shields.io/badge/arxiv-2015-green.svg" alt="paper" align="top"> 

<h4 id="distributed-quantum-compilation">Distributed Quantum Compilation</h4>

+ [DC-MBQC: A Distributed Compilation Framework for Measurement-Based Quantum Computing](https://arxiv.org/abs/2601.00214) Yecheng Xue et al <img src="https://img.shields.io/badge/arxiv-2026-green.svg" alt="paper" align="top">
+ [Optimizing Compilation for Distributed Quantum Computing via Clustering and Annealing](https://arxiv.org/abs/2508.15267) Ruilin Zhou et al <img src="https://www.google.com/search?q=https://img.shields.io/badge/QCE-2025-green.svg" alt="paper" align="top">
+ [A Modular Quantum Compilation Framework for Distributed Quantum Computing](https://arxiv.org/abs/2305.02969) Davide Ferrari et al <img src="https://img.shields.io/badge/TQE-2023-green.svg" alt="13-pages" align="top">
+ [Optimized Compiler for Distributed Quantum Computing](https://arxiv.org/abs/2112.14139) Daniele Cuomo et al <img src="https://img.shields.io/badge/TQC-2023-green.svg" alt="paper" align="top">
+ [Compiler Design for Distributed Quantum Computing](https://ieeexplore.ieee.org/document/9334411) Davide Ferrari et al <img src="https://img.shields.io/badge/TQE-2021-green.svg" alt="20-pages" align="top">

<h3 id="conference-and-journal">Conference and Journal</h3>

+ January - [ICCAD](https://www.iccad-conf.com/) [CCS](https://www.sigsac.org/ccs/CCS2026/)
+ March - [OOPSLA](https://2025.splashcon.org/track/OOPSLA) [TQC](https://tqc-conference.org/) [QCE](https://easychair.org/cfp/QCE25)
+ April - [QCE](https://qce.quantum.ieee.org/) [MICRO](https://www.microarch.org/)
+ July - [POPL](https://conf.researchr.org/home/POPL-2026)
+ August - [ASPLOS](https://www.asplos-conference.org/) <summer cycle>
+ September - [HPCA](https://hpca-conf.org/) [QIP](https://qipconference.org/)
+ November - [CC](https://conf.researchr.org/series/cc) [ISCA](https://iscaconf.org/) [PLDI](https://conf.researchr.org/series/pldi) [DAC](https://www.dac.com/) [CGO](https://2026.cgo.org/) [STOC](https://acm-stoc.org/) [ICSE](https://conf.researchr.org/home/icse-2026)

Impact Factor > 10
+ [Nature](https://www.nature.com/)
+ [Science](https://www.science.org/journal/science)
+ [Nature Machine Intelligence](https://www.nature.com/natmachintell/)
+ [Nature Physics](https://www.nature.com/nphys)  
+ [Nature Communications](https://www.nature.com/ncomms)
+ [PRX Quantum](https://journals.aps.org/prxquantum)
+ [Progress in Quantum Electronics](https://www.sciencedirect.com/journal/progress-in-quantum-electronics)

Impact Factor > 3
+ [Physical Review Letters](https://journals.aps.org/prl)
+ [IEEE TQE](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8780569)
+ [npj Quantum Information](https://www.nature.com/npjqi)
+ [ACM TQC](https://dl.acm.org/journal/tqc)
+ [Quantum](https://quantum-journal.org/)
+ [Quantum Science and Technology(QST)](https://iopscience.iop.org/journal/2058-9565)
+ [Quantum Machine Intelligence(QMI)](https://link.springer.com/journal/42484) 
+ [Advanced Quantum Technology(AQT)](https://onlinelibrary.wiley.com/journal/2511902X)

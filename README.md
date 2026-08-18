## Awesome Quantum Compiler 

<img src="https://awesome.re/badge-flat.svg" alt="Awesome" style="vertical-align: bottom;">

By studying [Quantum Compilation](https://arxiv.org/abs/2112.00187) written by Marco Maronese (2021) and [Quantum Compilation Process](https://link.springer.com/chapter/10.1007/978-3-031-90200-0_9) by Javier Cardama et al. (2025), as well as the classic [Nature Journal](https://www.nature.com/articles/nature23459) by Frederic T. Chong et al. (2017), we can get a clear sense of how to enter this field.

<h3 id="background-and-survey">Background and Survey</h3>

> Survey Paper

+ [Quantum Arithmetic Algorithms: Implementation, Resource Estimation, and Comparison](https://arxiv.org/abs/2509.07015) Dmytro Fedoriaka et al. (2025)
+ [Quantum Compiler Design for Qubit Mapping and Routing](https://arxiv.org/pdf/2505.16891) Chenghong zhu et al (2025).
+ [A Comprehensive Review of Quantum Circuit Optimization](https://www.mdpi.com/2624-960X/7/1/2) Krishnageetha Karuppasamy et al (2025).
+ [Quantum Circuit Synthesis and Compilation Optimization](https://arxiv.org/html/2407.00736v1) Ge Yan et al (2024).
+ [A Comprehensive Study of Quantum Arithmetic Circuits](https://arxiv.org/abs/2406.03867) Siyi Wang et al. (2024)



<h3 id="quantum-compilation">Quantum Compilation</h3>

+ [Two-bit gates are universal for quantum computation](https://arxiv.org/abs/cond-mat/9407022) D. P. DiVincenzo <img src="https://img.shields.io/badge/Citations-1000+-blue.svg"> (1994)
+ [Elementary gates for quantum computation](https://arxiv.org/abs/quant-ph/9503016) A. Barenco et al. <img src="https://img.shields.io/badge/Citations-4500+-blue.svg"> (1995)
+ [Optimal Quantum Circuits for General Two-Qubit Gates](https://arxiv.org/abs/quant-ph/0308006) Farrokh Vatan, Colin Williams <img src="https://img.shields.io/badge/Citations-580+-blue.svg"> (2003)
+ [Improved simulation of stabilizer circuits](https://arxiv.org/abs/quant-ph/0406196) Scott Aaronson, Daniel Gottesman <img src="https://img.shields.io/badge/Citations-2100+-blue.svg"> (2004)
+ [Synthesis of quantum-logic circuits](https://arxiv.org/abs/quant-ph/0406176) Vivek V. Shende et al. <img src="https://img.shields.io/badge/Citations-1000+-blue.svg"> (2004)
+ [An Introduction to Cartan’s KAK Decomposition for QC Programmers](https://arxiv.org/abs/quant-ph/0507171) Robert R. Tucci <img src="https://img.shields.io/badge/Citations-580+-blue.svg"> (2005)
+ [The Solovay-Kitaev algorithm](https://arxiv.org/abs/quant-ph/0505030) Christopher M. Dawson, Michael A. Nielsen <img src="https://img.shields.io/badge/Citations-900+-blue.svg"> (2005)

<h4 id="language-assembly-ir">PL, Assembly, and IR Design</h4>


+ [Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) Zhaohui Yang et al [[GitHub]](https://github.com/iqubit-org/phoenix) <img src="https://img.shields.io/badge/DAC-2025-green.svg">
+ [A QASM based Quantum Transpiler Framework for NISQ Devices](https://arxiv.org/abs/2308.07581) Fei Hua et al. [[Github]](https://github.com/pnnl/qasmtrans) <img src="https://img.shields.io/badge/SC-2023-green.svg">
+ [A Broader and Deeper Quantum Assembly Language](https://arxiv.org/abs/2104.14722) Andrew W. Cross et al. [[Github]](https://github.com/openqasm/openqasm) <img src="https://img.shields.io/badge/TQC-2022-green.svg">
+ [QSSA: An SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) Anurudh Peduri, Siddharth Bhat, Tobias Grosser [[GitHub]](https://github.com/opencompl/QMLIR)  <img src="https://img.shields.io/badge/CC-2022-green.svg">
+ [A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) David Ittah et al. [[GitHub]](https://github.com/dime10/QIRO) <img src="https://img.shields.io/badge/TQC-2022-green.svg">
+ [QRANE: Lifting QASM Programs to an Affine IR](https://dl.acm.org/doi/10.1145/3497776.3517775) Blake Gerard, Tobias Grosser, Martin Kong
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) Alexander McCaskey, Thien Nguyen <img src="https://img.shields.io/badge/QCE-2021-green.svg">
+ [An Open Source Software Framework for Quantum Computing](https://arxiv.org/abs/1612.08091) Damian S. Steiger et al. [[Github]](https://github.com/ProjectQ-Framework/ProjectQ) 
+ [PennyLane: Automatic differentiation of hybrid quantum-classical computations](https://arxiv.org/abs/1811.04968) Ville Bergholm et al. [[Github]](https://github.com/PennyLaneAI/pennylane) 
+ [Open Quantum Assembly Language](https://arxiv.org/abs/1707.03429) Andrew W. Cross et al. (2017) [[Github]](https://github.com/openqasm/openqasm)
+ [ScaffCC: Scalable Compilation and Analysis of Quantum Programs](https://arxiv.org/abs/1507.01902) Ali JavadiAbhari et al. [[GitHub]](https://github.com/epiqc/ScaffCC) <img src="https://img.shields.io/badge/CF-2015-green.svg"> 



<h4 id="hw-agnostic-compilation">HW-agnostic Circuit Compilation</h4>

+ [Optimizing Quantum Circuits, Fast and Slow](https://arxiv.org/pdf/2411.04104) Amanda Xu et al <img src="https://img.shields.io/badge/ASPLOS-2025-green.svg">
+ [Linear and non-linear relational analyses for Quantum Program Optimization](https://arxiv.org/abs/2410.23493) Matthew Amy, Joseph Lunderville <img src="https://img.shields.io/badge/POPL-2025-green.svg">
+ [Quantum Circuit Optimization for the Fault-Tolerance Era: Do We Have to Start from Scratch?](https://arxiv.org/abs/2509.02668) Tobias Forster et al. <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Optimizing Ancilla-Based Quantum Circuits with SPARE](https://dl.acm.org/doi/10.1145/3729253) Ritvik Sharma et al. <img src="https://img.shields.io/badge/PLDI-2025-green.svg">
+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) Francisco J. R. Ruiz [[GitHub]](https://github.com/google-deepmind/alphatensor_quantum) <img src="https://img.shields.io/badge/Nature Machine Intelligence-2025-green.svg">
+ [A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) Zikun Li et al. [[GitHub]](https://github.com/quantum-compiler/Quarl) [[Youtube]](https://youtu.be/DZjz88yDKC4?si=UTgp_1pQznhfs2Zs) <img src="https://img.shields.io/badge/OOPSLA-2024-green.svg"> 
+ [Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) Campbell et al. [[GitHub]](https://github.com/Infleqtion/client-superstaq) <img src="https://img.shields.io/badge/QCE-2023-green.svg">
+ [A Generalized Block-wise Compiler Optimization Framework for Quantum Simulation Kernels](https://arxiv.org/abs/2109.03371) Gushu Li et al. [[Youtube]](https://youtu.be/lXFVkBlh9_Q?si=y_d4SgUwWQPwerch) <img src="https://img.shields.io/badge/ASPLOS-2022-green.svg">
+ [Qubit Allocation](https://hal.science/hal-01655951/file/Siraichi_QubitAllocation_CGO18.pdf) Marcos Siraichi et al.  <img src="https://img.shields.io/badge/CGO-2018-green.svg"> 



<h4 id="hw-specific-compilation">HW-specific Compilation</h4>

> General

+ [On the Optimal Compilation for Fermion-to-Qubit Encoding](https://arxiv.org/pdf/2403.17794) Yuhao Liu et al. [[Github]](https://github.com/acasta-yhliu/fermihedral) [[Youtube]](https://www.youtube.com/watch?v=TLhNJRZUeas) <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg">
+ [AlphaRouter: Quantum Circuit Routing with Reinforcement Learning and Tree Search](https://arxiv.org/pdf/2410.05115) Wei Tang et al [[Github]](https://github.com/HYUIDSL/AlphaRouter) <img src="https://img.shields.io/badge/QCE-2024-green.svg">
+ [A Quantum Compiler for 2-local Qubit Hamiltonian Simulation Algorithms](arxiv.org/pdf/2108.02099) Lingling Lao, Dan E. Browne [[Github]](https://github.com/lllingoo/2QAN) [[Youtube]](https://www.youtube.com/watch?v=rBThLSpNpVU) <img src="https://img.shields.io/badge/ISCA-2022-green.svg">
+ [Qubit Mapping and Routing via MaxSAT](https://arxiv.org/abs/2208.13679v1) Abtin Molavi et al <img src="https://img.shields.io/badge/MICRO-2022-green.svg">
+ [A New Qubit Mapping Mechanism for Multi-programming Quantum Computing in Cloud Environment](https://ieeexplore.ieee.org/document/9407180) Lei Liu, Xinglei Dou <img src="https://img.shields.io/badge/HPCA-2021-green.svg">
+ [Time-optimal Qubit mapping](https://dl.acm.org/doi/pdf/10.1145/3445814.3446706) Chi Zhang et al. [[Youtube]](https://www.youtube.com/watch?v=_557jSReORo) <img src="https://img.shields.io/badge/ASPLOS-2021-green.svg">
+ [Tackling the Qubit Mapping Problem for NISQ-Era Quantum Devices](https://arxiv.org/abs/1809.02573) Gushu Li et al <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg"> 


> Superconducting + [[Google Quantum AI]](https://quantumai.google/research) [[IBM Quantum]](https://research.ibm.com/publications)

+ [Virtual-Z Gates and Symmetric Gate Compilation](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.6.020348) Arian Vezvaee et al <img src="https://img.shields.io/badge/APS-2025-green.svg">
+ [Direct Pulse-Level Compilation of Arbitrary Quantum Logic Gates on Superconducting Qutrits](https://arxiv.org/abs/2303.04261) Yujin Cho et al <img src="https://img.shields.io/badge/APS-2024-green.svg">
+ [A Time Optimization Framework for Robust and Low-Latency Quantum Circuits](https://arxiv.org/abs/2412.18533) Eduardo W. Lussi et al <img src="https://img.shields.io/badge/APS-2024-green.svg">
+ [Optimized Compilation of Aggregated Instructions for Realistic Quantum Computers](https://arxiv.org/pdf/1902.01474) Yunong Shi et al <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg">

> Trapped-Ion + [[Quantinuum]](https://www.quantinuum.com/research/research-areas#publications) [[IonQ]](https://www.ionq.com/publications)

+ [Shuttle & SWAP Co-Optimisation in QCCD](https://arxiv.org/abs/2505.01316) Chenghong Zhu et al <img src="https://img.shields.io/badge/ISCA-2025-green.svg">
+ [Graph-Based Pulse Representation for Diverse Quantum Control Hardware](https://arxiv.org/abs/2409.08407) Aniket S. Dalvi et al <img src="https://img.shields.io/badge/QCE-2024-green.svg">
+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) Francesco Preti <img src="https://img.shields.io/badge/Quantum-2024-green.svg">
+ [A Surface Code Compiler and Resource Estimator for Trapped-Ion Processors](https://dl.acm.org/doi/abs/10.1145/3624062.3624214) Tyler Leblond et al. [[Github]](https://github.com/ORNL-QCI/TISCC) <img src="https://img.shields.io/badge/SC-2023-green.svg"> 
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) Jonathan Durandau <img src="https://img.shields.io/badge/Quantum-2023-green.svg"> [[GitHub]](https://github.com/cda-tum/mqt-ion-shuttler)  
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) Fabian Kreppel et al <img src="https://img.shields.io/badge/Quantum-2022-green.svg">
+ [Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) Xin-Chuan Wu [[Youtube]](https://www.youtube.com/watch?v=SrcuokJUZp4) <img src="https://img.shields.io/badge/HPCA-2020-green.svg">
  
> Neutral atom + [[PasQal]](https://www.pasqal.com/publications/)

+ [A Retargetable Compiler Framework for FPQA Quantum Architectures](https://arxiv.org/pdf/2409.07870) Oğuzcan Kırmemiş et al. <img src="https://img.shields.io/badge/CGO-2025-green.svg">
+ [Enabling Concatenated Quantum Error Correction on Neutral Atom Arrays](https://arxiv.org/pdf/2508.05779) Pengyu Liu et al. <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Compiling quantum circuits for dynamically field-programmable neutral atoms array processors](https://arxiv.org/pdf/2306.03487.pdf) Bochen Tan et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg">
+ [Compiler Optimization for Bosonic Quantum Computing](https://arxiv.org/pdf/2402.02279) Junyu Zhou et al. <img src="https://img.shields.io/badge/ISCA-2024-green.svg">
+ [A Quantum Compiler for Reconfigurable Neutral Atom Arrays](https://arxiv.org/pdf/2311.15123) Hanrui Wang et al. [[Youtube]](https://www.youtube.com/watch?v=uTsOfMIm23s) <img src="https://img.shields.io/badge/ISCA-2024-green.svg">
+ [Pulse Family Optimization for Parametrized Quantum Gates Using Spectral Clustering](https://arxiv.org/abs/2408.00119) Robert de Keijzer et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg">
+ [Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) Hanrui Wang et al <img src="https://img.shields.io/badge/DAC-2024-green.svg">
+ [Compiling Quantum Circuits for Dynamically Field Programmable Neutral Atoms Array Processors](arxiv.org/pdf/2306.03487) Daniel Bochen Tan <img src="https://img.shields.io/badge/Quantum-2024-green.svg">
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) S. Ebadi et al <img src="https://img.shields.io/badge/Science-2022-green.svg">
+ [Qubit mapping for reconfigurable atom arrays](https://dl.acm.org/doi/abs/10.1145/3508352.3549331) Bochen Tan et al. [[Youtube]](https://youtu.be/-tr8KtDKKDU?si=l2SwrXNY3KWvLOPz) <img src="https://img.shields.io/badge/ICCAD-2022-green.svg">
+ [Optimal mapping for near-term quantum architectures based on Rydberg atoms](https://arxiv.org/abs/2109.04179) S.Brandhofer et al <img src="https://img.shields.io/badge/ICCAD-2021-green.svg">


> Photonics + [[PsiQuantum]](https://www.psiquantum.com/research)

+ [Adaptive Compilation for Resource-Constrained Photonic One-Way Quantum Computing](https://arxiv.org/abs/2504.17116) Hezi Zhang et al <img src="https://img.shields.io/badge/MICRO-2025-green.svg">
+ [A Scalable and Robust Compilation Framework for Emitter-Photonic Quantum Computing](https://arxiv.org/abs/2503.16346) Xiangyu Ren et al <img src="https://img.shields.io/badge/DAC-2025-green.svg">
+ [A Randomness-aware Compiler for Photonic Quantum Computing](https://arxiv.org/abs/2403.01829) Hezi Zhang et al [[Youtube]](https://www.youtube.com/watch?v=TLhNJRZUeas) <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg">
+ [Fusion-based quantum computation](https://arxiv.org/abs/2101.09310) Sara Bartolucci et al. <img src="https://img.shields.io/badge/PsiQuantum-bigTech-yellow.svg">
+ [A Compilation Framework for Photonic One-Way Quantum Computation](https://arxiv.org/abs/2209.01545) Hezi Zhang et al <img src="https://img.shields.io/badge/ISCA-2023-green.svg">
+ [A Compiler for Universal Photonic Quantum Computers](https://arxiv.org/abs/2210.09251) Felix Zilk et al <img src="https://img.shields.io/badge/QCS-2022-green.svg">


> Topolocial Quantum + [[Microsoft Quantum]([https://www.psiquantum.com/research](https://www.microsoft.com/en-us/research/research-area/quantum-computing/)]



<h4 id="compilation-with-error-mitigation">Compilation with error mitigation</h4>

+ [A Variational Approach to Quantum Error Mitigation](https://arxiv.org/abs/2112.05821) Gokul S. Ravi et al <img src="https://img.shields.io/badge/HPCA-2022-green.svg">
+ [Mitigating Idling Errors in Qubits via Adaptive Dynamical Decoupling](https://dl.acm.org/doi/10.1145/3466752.3480059) Poulami Das et al <img src="https://img.shields.io/badge/MICRO-2021-green.svg">
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503) Yongshan Ding et al <img src="https://img.shields.io/badge/MICRO-2020-green.svg">
+ [Digital Zero-Noise Extrapolation for Quantum Error Mitigation](https://arxiv.org/abs/2005.10921) Tudor Giurgica-Tiron et al <img src="https://img.shields.io/badge/QCE-2020-green.svg">
+ [Not All Qubits Are Created Equal: Variation-Aware Qubit Allocation in NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007) Swamit Tannu & Moinuddin Qureshi <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg">
+ [Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.](https://arxiv.org/abs/1901.11054) Prakash Murali et al. [[Github]](https://github.com/prakashmurali/TriQ) [[Youtube]](https://youtu.be/4RlOaxYPkX8?si=CieyhIebX3hjo6rj) <img src="https://img.shields.io/badge/ASPLOS-2019-green.svg" > 
+ [Practical Quantum Error Mitigation for Near-Future Applications](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509) Suguru Endo et al <img src="https://img.shields.io/badge/APS-2018-green.svg">
+ [Error Mitigation for Short-Depth Quantum Circuits](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509) Kristan Temme et al <img src="https://img.shields.io/badge/APS-2017-green.svg">

<h4 id="pulse-level-compilation">Pulse-level Compilation</h4>

+ [Towards a pulse-level intermediate representation for diverse quantum control systems](https://arxiv.org/abs/2507.15995) Jude Alnas et al. <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Tackling the Challenges of Adding Pulse-level Support to a Heterogeneous HPCQC Software Stack: MQSS Pulse](https://dl.acm.org/doi/10.1145/3731599.3767552) Jorge Echavarria et al. <img src="https://img.shields.io/badge/SC-2025-green.svg">
+ [Enhancing Noisy Quantum Sensing by GHZ State Partitioning](https://arxiv.org/pdf/2507.02829) Allen Zang et al. <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Variational Quantum Pulse Learning](https://arxiv.org/abs/2203.17267) Zhiding Liang et al. <img src="https://img.shields.io/badge/QCE-2022-green.svg">
+ [Enabling Pulse-Level Programming, Compilation, and Execution in XACC](https://arxiv.org/pdf/2003.11971) Thien Nguyen, Alexander McCaskey [[Github]](https://github.com/eclipse/xacc) <img src="https://img.shields.io/badge/TC-2020-green.svg">
+ [Resource-Efficient Quantum Computing by Breaking Abstractions](https://arxiv.org/abs/2011.00028) Yunong Shi <img src="https://img.shields.io/badge/IEEE-2020-green.svg">
+ [Optimized Quantum Compilation for Near-Term Algorithms with OpenPulse](https://arxiv.org/abs/2004.11205) Pranav Gokhale et al. [[Github]](https://github.com/singular-value/optimizations_via_openpulse) [[Youtube]](https://youtu.be/dtPaDmE89Yc?si=5z1tfMK7FSw-SRsw) 
+ [Software Mitigation of Crosstalk on Noisy Intermediate-Scale Quantum Computers](https://arxiv.org/pdf/2001.02826) Prakash Murali et al. <img src="https://img.shields.io/badge/ASPLOS-2020-green.svg">
+ [Partial Compilation of Variational Algorithms for Near-term Quantum Machines](https://arxiv.org/pdf/1909.07522) Pranav Gokhale et al. [[Github]](https://github.com/epiqc/PartialCompilation) <img src="https://img.shields.io/badge/MICRO-2019-green.svg">


<h4 id="qec-aware compilation">QEC-aware compilation</h4>

+ [In-situ Qubit Calibration for Surface Code Quantum Error Correction](https://dl.acm.org/doi/pdf/10.1145/3695053.3731042) <img src="https://img.shields.io/badge/ISCA-2025-green.svg">
+ [A Resource-Allocating Compiler for Lattice Surgery](https://arxiv.org/abs/2506.04620) Alan Robertson et al. [[GitHub]](https://github.com/latticesurgery-com/lattice-surgery-compiler)<img src="https://img.shields.io/badge/QCS-2025-green.svg"> 
+ [Dependency-Aware Compilation for Surface Code Quantum Architectures](https://arxiv.org/abs/2311.18042) Abtin Molavi et al. <img src="https://img.shields.io/badge/OOPSLA-2025-green.svg">
+ [QEC on Demand via In-Situ Encoding of Bare Qubits for Ion Trap Architectures](https://arxiv.org/abs/2504.16303) Keyi Yin et al. 
+ [Efficient Circuit Mapping and Scheduling for Surface Code](https://arxiv.org/abs/2312.15254) Mingzheng Zhu et al. <img src="https://img.shields.io/badge/CGO-2024-green.svg">
+ [A New Routing Strategy to Improve Success Rates of Quantum Circuits](https://dl.acm.org/doi/pdf/10.1145/3649476.3658790) Lu Fang et al <img src="https://img.shields.io/badge/ICCAD-2024-green.svg">
+ [Optimizing FTQC Programs through QEC Transpiler and Architecture Codesign](https://arxiv.org/abs/2412.15434) Meng Wang et al. <img src="https://img.shields.io/badge/TACO-2024-green.svg">
+ [A High Performance Compiler for Very Large Scale Surface Code Computations](https://arxiv.org/abs/2302.02459) George Watkins et al <img src="https://img.shields.io/badge/Quantum-2024-green.svg">
+ [Realistic Cost to Execute Practical Quantum Circuits using Direct Clifford+T Lattice Surgery Compilation](https://arxiv.org/abs/2311.10686) Tyler LeBlond et al. [[Github]](https://github.com/ORNL-QCI/TISCC) <img src="https://img.shields.io/badge/TQC-2024-green.svg">
+ [An architecture for efficient fault-tolerant quantum computers with limited non-local connections](https://arxiv.org/abs/2211.15465) Daniel Litinski, Naomi Nickerson <img src="https://img.shields.io/badge/PsiQuantum-bigTech-yellow.svg">
+ [A Framework for Enabling Efficient Surface Code Communication in Quantum Computing](https://dl.acm.org/doi/10.1145/3466752.3480072) Fei Hua et al. <img src="https://img.shields.io/badge/MICRO-2021-green.svg">


<h3 id="fault-tolerant-quantum-computing">Fault-Tolerant Quantum Computing</h3>

+ [Fault-tolerant quantum computation](https://arxiv.org/abs/quant-ph/9605011) Peter Shor <img src="https://img.shields.io/badge/Citations-1700+-blue.svg"> (1996)
+ [Fault-tolerant quantum computation by anyons](https://arxiv.org/abs/quant-ph/9707021) Alexei Kitaev <img src="https://img.shields.io/badge/Citations-10000+-blue.svg"> (1997)
+ [Resilient Quantum Computation](https://arxiv.org/abs/quant-ph/9702058) Emanuel Knill et al <img src="https://img.shields.io/badge/Citations-670+-blue.svg"> (1998)
+ [Theory of fault-tolerant quantum computation](https://arxiv.org/abs/quant-ph/9702029) Daniel Gottesman <img src="https://img.shields.io/badge/Citations-1300+-blue.svg"> (1998)
+ [Fault-Tolerant Quantum Computation with Constant Error Rate](https://arxiv.org/abs/quant-ph/9906129) Dorit Aharonov, Michael Ben-Or <img src="https://img.shields.io/badge/Citations-1700+-blue.svg"> (1999) 
+ [A One-Way Quantum Computer](https://arxiv.org/abs/quant-ph/0108118) Raussendorf and Briegel <img src="https://img.shields.io/badge/Citations-5900+-blue.svg"> (2001)
+ [Universal quantum computation with ideal Clifford gates and noisy ancillas](https://arxiv.org/abs/quant-ph/0403025) Bravyi and Kitaev <img src="https://img.shields.io/badge/Citations-2200+-blue.svg"> (2005)
+ [Fault-Tolerant Quantum Computation with High Threshold in Two Dimensions](https://arxiv.org/abs/quant-ph/0610082) Raussendorf et al. <img src="https://img.shields.io/badge/Citations-1100+-blue.svg"> (2007)
  
<h4 id="magic-state-factory">Magic State Factory</h4>

+ [Constant-overhead magic state distillation](https://arxiv.org/abs/2408.07764) Adam Wills et al. <img src="https://img.shields.io/badge/Nature-2024-green.svg"> 
+ [Experimental demonstration of logical magic state distillation](https://arxiv.org/abs/2412.15165) Pedro Sales Rodriguez et al. <img src="https://img.shields.io/badge/Nature-2024-green.svg"> 
+ [Encoding a magic state with beyond break-even fidelity](https://arxiv.org/abs/2305.13581) Riddhi S. Gupta et al. <img src="https://img.shields.io/badge/Nature-2023-green.svg"> 
+ [Magic state cultivation: growing T states as cheap as CNOT gates](https://arxiv.org/abs/2409.17595) Craig Gidney et al. 
+ [Logical Magic State Preparation with Fidelity beyond the Distillation Threshold on a Superconducting Quantum Processor](https://arxiv.org/abs/2305.15972) Yangsen Ye et al. <img src="https://img.shields.io/badge/APS-2023-green.svg"> 
+ [Unfolded distillation: very low-cost magic state preparation for biased-noise qubits](https://www.nature.com/articles/s41534-026-01197-z) Diego Ruiz et al. <img src="https://img.shields.io/badge/npj Quantum-2023-green.svg"> 
+ [Locality-Aware Pauli-Based Computation for Local Magic State Preparation](https://arxiv.org/abs/2504.12091) Keita Kanno et al <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Magic state distillation: Not as costly as you thin](https://arxiv.org/abs/1905.06903) Daniel Litinski <img src="https://img.shields.io/badge/Quantum-2019-green.svg">
+ [Mapping and scheduling multi-level distillation circuits for fault-tolerant quantum architectures](https://dl.acm.org/doi/10.1109/MICRO.2018.00072) Yongshan Ding et al. <img src="https://img.shields.io/badge/MICRO-2018-green.svg">
+ [Quantum computation with realistic magic-state factories](https://arxiv.org/abs/1605.07197) Joe O'Gorman, Earl T. Campbell <img src="https://img.shields.io/badge/APS-2017-green.svg">


<h4 id="resource-estimation">Resource Estimation</h4> 

+ [[Gidney Google Scholar]](https://scholar.google.com/citations?user=qKTv84IAAAAJ&hl=en) + [[Gidney Blog]](https://algassert.com/)
+ [Resource Analysis of Low-Overhead Transversal Architectures for Reconfigurable Atom Arrays](https://arxiv.org/abs/2505.15907) Hengyun Zhou et al. <img src="https://img.shields.io/badge/ISCA-2025-green.svg">
+ [Quantum resource estimation for large scale quantum algorithms](https://www.sciencedirect.com/science/article/pii/S0167739X24004308) Vlad Gheorghiu and Michele Mosca <img src="https://img.shields.io/badge/Future Generation Computer Systems-2025-green.svg">
+ [How to factor 2048-bit RSA integers in 8 hours using 20 million noisy qubits](https://quantum-journal.org/papers/q-2021-04-15-433/) Craig Gidney and Martin Eke  <img src="https://img.shields.io/badge/Quantum-2021-green.svg">
+ [Factoring 2048-bit RSA Integers in 177 Days with 13 436 Qubits and a Multimode Memory](https://arxiv.org/abs/2103.06159) Élie Gouzien and Nicolas Sangouard <img src="https://img.shields.io/badge/APS-2021-green.svg">
+ [Efficient magic state factories with a catalyzed |CCZ⟩ to 2|T⟩ transformation](https://arxiv.org/abs/1812.01238) Craig Gidney, Austin G. Fowler <img src="https://img.shields.io/badge/Quantum-2019-green.svg">
+ [Large-Scale Quantum Computing with Lattice Surgery](https://arxiv.org/abs/1808.02892) Daniel Litinski <img src="https://img.shields.io/badge/Quantum-2019-green.svg">
+ [Windowed Quantum Arithmetic](https://arxiv.org/abs/1905.07682) Craig Gidney (2019)


<h4 id="distributed-ft-compilation">Distributed Quantum Computing</h4>

+ [A Distributed Compilation Framework for Measurement-Based Quantum Computing](https://arxiv.org/abs/2601.00214) Yecheng Xue et al <img src="https://img.shields.io/badge/HPCA-2025-green.svg">
+ [Optimizing Distributed Quantum Computing for Quantum Data Centers with Switch Networks]() Hezi Zhang et al. <img src="https://img.shields.io/badge/ISCA-2025-green.svg">
+ [Optimizing Compilation for Distributed Quantum Computing via Clustering and Annealing](https://arxiv.org/abs/2508.15267) Ruilin Zhou et al <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Multi-Entry Communication Highway for Superconducting Quantum Chiplets](https://arxiv.org/abs/2305.05149) Hezi Zhang et al. <img src="https://img.shields.io/badge/ASPLOS-2024-green.svg">
+ [Qubit Allocation for Distributed Quantum Computing](https://ieeexplore.ieee.org/document/10228915) Yingling Mao et al <img src="https://img.shields.io/badge/INFOCOM-2023-green.svg">
+ [Modular architectures for fault-tolerant photonic quantum computing](https://arxiv.org/abs/2103.08612) Héctor Bombín et al. <img src="https://img.shields.io/badge/PsiQuantum-bigTech-yellow.svg">


<h4 id="compiler-level-quantum-cryptanalysis">Compiler-level Quantum Cryptanalysis</h4>

+ [[Survey] Quantum Cryptanalysis: Shor, Grover, and Beyond](https://nist.pqcrypto.org/foia/20240215/Re_%20WERB(1)_2.pdf-attachment-cryptanalysis.pdf) 
+ [Factoring using 2n+2 qubits with Toffoli based modular multiplication](https://arxiv.org/abs/1611.07995) Thomas Häner et al. <img src="https://img.shields.io/badge/QIC-2016-green.svg">
+ [Optimal ancilla-free Clifford+T approximations of z-rotations](https://arxiv.org/abs/1403.2975) Neil J. Ross et al. <img src="https://img.shields.io/badge/QIC-2014-green.svg">
+ [An algorithm for the T-count](https://arxiv.org/abs/1308.4134) David Gosset et al. <img src="https://img.shields.io/badge/QIC-2014-green.svg">
+ [Faster Quantum Number Factoring via Circuit Synthesis](https://arxiv.org/abs/1301.3210) Igor L. Markov et al. <img src="https://img.shields.io/badge/APS-2013-green.svg">
+ [Polynomial-time T-depth Optimization of Clifford+T circuits via Matroid Partitioning](https://arxiv.org/abs/1303.2042) Matthew Amy et al. <img src="https://img.shields.io/badge/TCAD-2013-green.svg">
+ [A meet-in-the-middle algorithm for fast synthesis of depth-optimal quantum circuits](https://arxiv.org/abs/1206.0758) Matthew Amy et al. <img src="https://img.shields.io/badge/TCAD-2012-green.svg">
+ [Fast Quantum Modular Exponentiation Architecture for Shor's Factorization Algorithm Archimedes](https://arxiv.org/abs/1207.0511) Pavlidis et al. <img src="https://img.shields.io/badge/QIC-2012-green.svg">
+ [Constant-Optimized Quantum Circuits for Modular Multiplication and Exponentiation](https://arxiv.org/abs/1202.6614) Igor L. Markov et al. <img src="https://img.shields.io/badge/QIC-2012-green.svg">
+ [A quantum circuit for Shor's factoring algorithm using 2n+2 qubits](https://dl.acm.org/doi/abs/10.5555/2011665.2011669) Y. Takahashi et al. <img src="https://img.shields.io/badge/QIC-2006-green.svg">
+ [Fast quantum modular exponentiation](https://arxiv.org/abs/quant-ph/0408006) Rodney Van Meter et al. <img src="https://img.shields.io/badge/APS-2005-green.svg">
+ [Implementation of Shor's Algorithm on a Linear Nearest Neighbour Qubit Array](https://arxiv.org/abs/quant-ph/0402196) Andrew G. Fowler <img src="https://img.shields.io/badge/QIC-2004-green.svg">
+ [Circuit for Shor's algorithm using 2n+3 qubits](https://arxiv.org/abs/quant-ph/0205095) Stéphane Beauregard <img src="https://img.shields.io/badge/QIC-2003-green.svg">


<h4 id="compiler-level-pqc">Compiler-level Quantum Cryptography</h4>  

> My experiences I went through during my past year at university <br>
inspired me to decide to pursue research on PQC as well

+ [[Survey] Post-Quantum Cryptography and Quantum-Safe Security: A Comprehensive Survey](https://arxiv.org/abs/2510.10436)
+ [Automatic Large-Scale Constant-Time Analysis](https://arxiv.org/pdf/2501.04183) Zhiyuan Zhang, Gilles Barthe <img src="https://img.shields.io/badge/OOPSLA-2026-green.svg">
+ [Decompiling for Constant-Time Analysis](https://arxiv.org/abs/2501.04183) Santiago Arranz-Olmos et al. <img src="https://img.shields.io/badge/OOPSLA-2026-green.svg">
+ [How Compilers Break and Fix Constant-Time Code](https://arxiv.org/abs/2507.06112) Antoine Geimer, Clementine Maurice <img src="https://img.shields.io/badge/IACR-2025-green.svg">
+ [How Compilers Break Constant-Time Implementations](https://arxiv.org/abs/2410.13489) Moritz Schneider et al. <img src="https://img.shields.io/badge/CCS-2025-green.svg">
+ [Smooth, Integrated Proofs of Cryptographic Constant Time for Nondeterministic Programs and Compilers](https://arxiv.org/abs/2504.15550) Owen Conoly et al. <img src="https://img.shields.io/badge/PLDI-2025-green.svg">
+ [Preservation of Speculative Constant-Time by Compilation](https://dl.acm.org/doi/10.1145/3704880) Santiago Arranz Olmos et al. <img src="https://img.shields.io/badge/POPL-2024-green.svg">
+ [Vectorized Implementation of Kyber and Dilithium on 32-bit Cortex-A Series](https://ieeexplore.ieee.org/document/10614163/) Youngbeom Kim et al. <img src="https://img.shields.io/badge/IEEE-2024-green.svg">
+ [Optimized Software Implementation of Keccak, Kyber, and Dilithium on RISC-V](https://eprint.iacr.org/2024/1515) Jipeng Zhang et al. <img src="https://img.shields.io/badge/IACR-2024-green.svg">
+ [Faster Post-Quantum TLS 1.3 Based on ML-KEM: Implementation and Assessment](https://arxiv.org/abs/2404.13544) Jieyu Zheng et al. <img src="https://img.shields.io/badge/IACR-2024-green.svg">
+ [Machine-checked IND-CCA security and correctness of ML-KEM in EasyCrypt](https://eprint.iacr.org/2024/843) José Bacelar Almeida et al. <img src="https://img.shields.io/badge/IACR-2024-green.svg">
+ [Optimized Vectorization Implementation of CRYSTALS-Dilithium](https://arxiv.org/abs/2306.01989) Jieyu Zheng et al. <img src="https://img.shields.io/badge/CRYPTO-2023-green.svg">
+ [Faster Kyber and Dilithium on the Cortex-M4](https://eprint.iacr.org/2022/112) Amin Abdulrahman et al. <img src="https://img.shields.io/badge/IACR-2022-green.svg"> [Github](https://github.com/FasterKyberDilithiumM4/FasterKyberDilithiumM4)
+ [Faster Dilithium, Kyber, and Saber on Cortex-A72 and Apple M1](https://eprint.iacr.org/2021/986) Hanno Becker et al. <img src="https://img.shields.io/badge/IACR-2021-green.svg"> [Github](https://github.com/neon-ntt/neon-ntt)
+ [Compact Implementations of Kyber on 64-bit ARM Cortex-A Processors](https://eprint.iacr.org/2021/561) Pakize Sanal et al. <img src="https://img.shields.io/badge/IACR-2021-green.svg">
+ [Memory-Efficient High-Speed Implementation of Kyber on Cortex-M4](https://eprint.iacr.org/2019/489) Leon Botros et al. <img src="https://img.shields.io/badge/IACR-2019-green.svg">
+ [Formal Verification of a Constant-Time Preserving C Compiler](https://dl.acm.org/doi/10.1145/3371075) Gilles Barthe et al. <img src="https://img.shields.io/badge/POPL-2019-green.svg">


</br>

<h3 id="quantum-system-software-infrastructure">Quantum System Software Infrastructure</h3>

<h4 id="quantum-testing-and-debugging">Quantum Testing and Debugging</h4>

+ [[Survey] Testing and Debugging Quantum Programs: The Road to 2030](https://dl.acm.org/doi/10.1145/3715106) Neilson Carlos Leite Ramalho et al. 
+ [Automated Testing of Quantum Programs with Complex Input States](https://dl.acm.org/doi/10.1109/ASE56229.2023.00196) Jiaming Ye et al. [[Github]](https://github.com/ToolmanInside/quratest-mutators) <img src="https://img.shields.io/badge/ASE-2023-green.svg">
+ [Metamorphic Testing for Quantum Programs](https://arxiv.org/abs/2206.01111) Matteo Paltenghi, Michael Pradel [[Github]](https://github.com/sola-st/MorphQ-Quantum-Qiskit-Testing-ICSE-23) <img src="https://img.shields.io/badge/ICSE-2023-green.svg"> 
+ [Quantum Combinatorial Testing Framework](https://arxiv.org/abs/2309.00119) Xinying Wang et al. [[Youtube]](https://www.youtube.com/watch?v=UsqgOudKLio) <img src="https://img.shields.io/badge/ASE-2023-green.svg">
+ [Search-Based Testing of Quantum Programs](https://dl.acm.org/doi/10.1145/3510454.3516839) Xinying Wang et al. [[Youtube]](https://www.youtube.com/watch?v=Wh0FZ-kTglo) <img src="https://img.shields.io/badge/ICSE-2022-green.svg"> 
+ [A Mutation Testing Tool for Quantum Algorithms and Applications in Qiskit](https://jose.github.io/assets/pdfs/ISSTA2022-tool-paper.pdf) E. Fortunato et al. [[Github]](https://github.com/jose/qmutpy-experiments) <img src="https://img.shields.io/badge/ASE-2022-green.svg">
+ [A coverage-guided test generator for quantum programs](https://dl.acm.org/doi/abs/10.1109/ASE51524.2021.9678798) Xinyi Wang et al. [[Github]](https://github.com/Simula-COMPLEX/quito) [[Youtube]](https://www.youtube.com/watch?v=kuI9QaCo8A8)  <img src="https://img.shields.io/badge/ASE-2021-green.svg">
+ [Mutation Testing for Qiskit Quantum Programs](https://ieeexplore.ieee.org/document/9678563) A. Mendiluze et al. [[Github]](https://github.com/Simula-COMPLEX/muskit) <img src="https://img.shields.io/badge/ASE-2021-green.svg"> 
+ [Projection-based runtime assertions for testing and debugging Quantum programs](https://dl.acm.org/doi/10.1145/3428218) Gushu Li et al. [[Youtube]](https://www.youtube.com/watch?v=7GVNWMR1NX4) <img src="https://img.shields.io/badge/OOPSLA-2020-green.svg"> 
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/pdf/1810.00375) Thomas Häner et al <img src="https://img.shields.io/badge/OOPSLA-2020-green.svg">
+ [Statistical Assertions for Quantum Programs](https://arxiv.org/abs/1905.09721) Yipeng Huang, M. Martonosi [[Youtube]](https://www.youtube.com/watch?v=Jic3OcJHmRg)  <img src="https://img.shields.io/badge/ISCA-2019-green.svg">


<h4 id="quantum-formal-verification">Quantum Formal Verification</h4>

+ [Efficient Formal Verification of Quantum Error Correcting Programs](https://arxiv.org/abs/2504.07732) Qifan Huang et al. <img src="https://img.shields.io/badge/PLDI-2025-green.svg"> 
+ [Quantum Correctness by Construction](https://arxiv.org/abs/2307.15641) Anurudh Peduri et al. <img src="https://img.shields.io/badge/OOPSLA-2025-green.svg">
+ [Symbolic Execution for Quantum Error Correction Programs](https://arxiv.org/pdf/2311.11313) Wang Fang, Mingsheng Ying. <img src="https://img.shields.io/badge/PLDI-2024-green.svg"> 
+ [Quantum Probabilistic Model Checking for Time-Bounded Properties](https://dl.acm.org/doi/10.1145/3689731) Seungmin Jeon et al. <img src="https://img.shields.io/badge/OOPSLA-2024-green.svg">
+ [A Design of Software Architecture for Validate and Verification of Linear-Optical Quantum Computing Platform](https://ieeexplore.ieee.org/document/10313808) Duwon Lee et al <img src="https://img.shields.io/badge/QCE-2023-green.svg">
+ [Foundational Verification of Quantum Programs](https://arxiv.org/abs/2207.11350) L. Zhou [[Youtube]](https://www.youtube.com/watch?v=RjKCP8U-1Zg) <img src="https://img.shields.io/badge/POPL-2022-green.svg"> 
+ [Sound Reasoning for Purity and Entanglement in Quantum Programs](https://arxiv.org/abs/2205.02287) Charles Yuan et al [[Github]](https://github.com/psg-mit/twist-popl22)[[Youtube]](https://www.youtube.com/watch?v=H3GIBgH5Ud4) <img src="https://img.shields.io/badge/POPL-2022-green.svg">
+ [Push-Button Verification for the Qiskit Quantum Compiler](https://arxiv.org/pdf/2205.00661) Runzhou Tao at al. [[Github]](https://github.com/taorunz/Giallar) [[Youtube]](https://www.youtube.com/watch?v=m9pR53Zcj5w) <img src="https://img.shields.io/badge/PLDI-2022-green.svg"> 
+ [Quantum Relational Hoare Logic](https://arxiv.org/abs/1802.03188) Dominique Unruh [[Youtube]](https://www.youtube.com/watch?v=U1-xP2SMDc0) <img src="https://img.shields.io/badge/POPL-2019-green.svg">
+ [A Core Language for Quantum Circuits](https://dl.acm.org/doi/10.1145/3009837.3009894) J. Paykin et al [[Github]](https://github.com/inQWIRE/QWIRE) <img src="https://img.shields.io/badge/POPL-2017-green.svg"> 

<h4 id="quantum-secure-compilation">Quantum Secure Compilation</h4>

+ [Program Output Obfuscation for Quantum Software Circuits in Quantum Clouds](https://hpcrl.github.io/ICS2025-webpage/program/ICS25/ics25-32.pdf) Tirthak Patel et al <img src="https://img.shields.io/badge/ICS-2025-green.svg">
+ [Quantum Circuit Split Compilation with Interlocking Patterns](https://arxiv.org/abs/2503.11982) Qian Wang et al <img src="https://img.shields.io/badge/DAC-2025-green.svg">  
+ [Enhanced locking for quantum circuit IP protection](https://arxiv.org/abs/2412.17101) Y Liu et al <img src="https://img.shields.io/badge/QCE-2025-green.svg">
+ [Obfuscating quantum hybrid-classical algorithms for security and privacy](https://arxiv.org/abs/2305.02379) S Upadhyay, S Ghosh <img src="https://img.shields.io/badge/QCE-2024-green.svg">
+ [Leveraging Quantum Circuit Cutting for Obfuscation and Intellectual Property Protection](https://arxiv.org/pdf/2511.04842) G Typaldos, W Tang, J Szefer <img src="https://img.shields.io/badge/QCE-2024-green.svg">
+ [Split Compilation for Security of Quantum Circuits](https://pure.psu.edu/en/publications/split-compilation-for-security-of-quantum-circuits) Abdullah Ash Saki et al <img src="https://img.shields.io/badge/ICCAD-2021-green.svg">

<h4 id="quantum-os">Quantum Operating System</h4>

+ [An Operating System For Executing Applications On Quantum Network Nodes](https://www.nature.com/articles/s41586-025-08704-w) C. Delle Donne et al. <img src="https://img.shields.io/badge/Nature-2025-green.svg">
+ [A Quantum Operating System](https://arxiv.org/abs/2406.19120) Emmanouil Giortamis et al. <img src="https://img.shields.io/badge/OSDI-2025-green.svg"> 
+ [An Open-Source Hybrid Quantum Operating System](https://arxiv.org/abs/2308.06313) Stavros Efthymiou et al. [[Github]](https://github.com/qiboteam/qibolab) <img src="https://img.shields.io/badge/Quantum-2025-green.svg">
+ [Quantum Operating Systems](https://people.eecs.berkeley.edu/~henrycg/files/academic/papers/hotos17quantum.pdf) Henry Corrigan-Gibbs et al <img src="https://img.shields.io/badge/HotOS-2017-green.svg">

<h3 id="conference-deadline">Top Conference Deadline</h3>

+ January - [ICCAD](https://www.iccad-conf.com/) [CCS](https://www.sigsac.org/ccs/CCS2026/) 
+ March - [OOPSLA](https://2025.splashcon.org/track/OOPSLA) [TQC](https://tqc-conference.org/) [QCE](https://easychair.org/cfp/QCE25)
+ April - [QCE](https://qce.quantum.ieee.org/) [MICRO](https://www.microarch.org/)
+ July - [POPL](https://conf.researchr.org/home/POPL-2026)
+ August - [ASPLOS](https://www.asplos-conference.org/) <summer cycle>
+ September - [HPCA](https://hpca-conf.org/) [QIP](https://qipconference.org/)
+ November - [CC](https://conf.researchr.org/series/cc) [ISCA](https://iscaconf.org/) [PLDI](https://conf.researchr.org/series/pldi) [DAC](https://www.dac.com/) [CGO](https://2026.cgo.org/) [STOC](https://acm-stoc.org/) [ICSE](https://conf.researchr.org/home/icse-2026)
+ CrytoSystem - [Journal of Cryptology](https://www.iacr.org/jofc/) [IACR](https://eprint.iacr.org/)



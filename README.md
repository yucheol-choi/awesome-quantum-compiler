# Awesome-Quantum-Compilers

0. Quantum Compilation Surveys
1. Front-end & High-level IR
   1a. Languages & IR design (QASM, Program Synthesis, High-level Abstraction)
   1b. Loop & program transforms
   1c. Circuit Analysis (static metrics, cost models)
2. Middle-end Optimisations & Scheduling
   2a. Quantum Circuit Scheduling (gate/cycle level)
   2b. Gate/Cycle Scheduling. Logic-level (depth, T-count, synthesis)
   2c. Layout-level passes (mapping, SWAP, connectivity, partitioning)
3. Back-end & Hardware Execution / Runtime
   3a. Cycle/Gate Scheduling (ISA layer)
   3b. Control-level (pulse scheduling, optimal control)
   3c. Runtime & ISA (Hardware-aware compilation, Quantum ISA)
   측정 결과에 따른 실시간 분기나 feedforward 제어는 런타임 단계에서 중요성이 커지고 있어 (dynamic circuit)
   LLVM MLIR 기반의 qe-compiler처럼 하드웨어 특성에 맞춘 코드 생성·실행 모듈
4. Verification & Benchmark / Simul & Debug 
전체 파이프라인 신뢰성을 확보하기 위한 후처리 단계
   4a. Verification & Benchmark
   4b. Evaluation & Simulation 
   4c. Debug & Test 

5. Error Mitigate and Correction

Gate/Cycle Scheduling
연산 횟수 및 회로 깊이를 줄여 노이즈 민감도를 낮추는 작업

LLVM MLIR 기반의 qe-compiler처럼 하드웨어 특성에 맞춘 코드 생성·실행 모듈

#### Quantum Compilation Surveys
+ [Quantum Compilation Process: A Survey](https://link.springer.com/chapter/10.1007/978-3-031-90200-0_9) - F. Javier Cardama, Jorge Vázquez-Pérez, Tomás F. Pena, Juan C. Pichel & Andrés Gómez, 2025
+ [Quantum Compiler Design for Qubit Mapping and Routing](https://arxiv.org/pdf/2505.16891) - Chenghong zhu et al., 2025.
+ [A Comprehensive Review of Quantum Circuit Optimization: Current Trends and Future Directions](https://www.mdpi.com/2624-960X/7/1/2) - Krishnageetha Karuppasamy et al., 2025.
+ [Quantum Circuit Synthesis and Compilation Optimization: Overview and Prospects](https://arxiv.org/html/2407.00736v1) - Ge Yan et al., 2024.
+ [Quantum Compiling](https://arxiv.org/abs/2112.00187) - Marco Maronese, Lorenzo Moro, Lorenzo Rocutto, Enrico Prati, 2021
+ [Quantum compiling by deep reinforcement learning](https://www.nature.com/articles/s42005-021-00684-3) - Lorenzo Moro, Matteo G. A. Paris, Marcello Restelli, Enrico Prati, Nature, 2021
+ [Programming languages and compiler design for realistic quantum hardware](https://www.nature.com/articles/nature23459) - Frederic T. Chong, Diana Franklin, Margaret Martonosi, Nature, 2017
</br>


### Front-end IR & High-Level IR 
+ [LinguaQuanta: Towards a Quantum Transpiler Between OpenQASM and Quipper](https://arxiv.org/pdf/2404.08147) - Scott Wesley, 2024.
+ [Design and synthesis of scalable quantum programs](https://arxiv.org/abs/2412.07372) - Tomer Goldfriend et al., 2025.
+ [PHOENIX: Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) - Zhaohui Yang et al.,2025.
+ [Practical and efficient quantum circuit synthesis and transpiling with Reinforcement Learning](https://arxiv.org/abs/2405.13196) - David Kremer et al.,2025.
+ [Qmod: Expressive High-Level Quantum Modeling]([Matan Vax](https://arxiv.org/html/2502.19368v1) - Matan Vax et al., 2025. 
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) - David Ittah, Thomas Häner, Vadym Kliuchnikov, Torsten Hoefler, ACM Transactions on Quantum Computing, 2021.
+ [A Cross-Platform Execution Engine for the Quantum Intermediate Representation](https://arxiv.org/pdf/2404.14299) - Elaine Wong et al., 2024
+ [InQuIR: Intermediate Representation for Interconnected Quantum Computers](https://arxiv.org/abs/2302.00267) - Shin Nishio, Ryo Wakizaka, 2023
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) - Anurudh Peduri, Siddharth Bhat, CC, 2022
+ [Quantum circuit transformations with a multi-level intermediate representation compiler](https://arxiv.org/abs/2112.10677) - T. Nguyen et al., 2021
+ [Enabling Retargetable Optimizing Compilers for Quantum Accelerators via a Multi-Level Intermediate Representation](https://arxiv.org/abs/2109.00506) - Thien Nguyen, Alexander McCaskey, 2021
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) - Alexander McCaskey, Thien Nguyen, QCE, 2021
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) - Ali JavadiAbhari, Shruti Patil, Daniel Kudrow, Jeff Heckey, Alexey Lvov, Frederic T. Chong, Margaret Martonosi, Parallel Comput, CF, 2014
+ [Introducing Quantum Intermediate Representation (QIR)](https://devblogs.microsoft.com/qsharp/introducing-quantum-intermediate-representation-qir/)

#### Loop & Program Transforms ####
+ [Thoughts on Adopting the Quantum Intermediate Representation (QIR)](https://arxiv.org/pdf/2411.18682) – Ynnick Stade et al., 2024
+ [The Limits of Control Flow in Quantum Programming](https://arxiv.org/abs/2304.15000) – Charles Yuan, Agnes Villanyi, Michael Carbin, 2023
+ [Software Pipelining for Quantum Loop Programs](https://arxiv.org/abs/2012.12700) – Jingzhe Guo, Mingsheng Ying, IEEE TSE, 2023. 
+ [Exploring the Impact of Affine Loop Transformations in Qubit Allocation](https://arxiv.org/pdf/2010.11999) - Martin Kong, 2020.

#### Quantum Circuit Analysis #### 
+ [Character Complexity: A Novel Measure for Quantum Circuit Analysis](https://arxiv.org/abs/2408.09641) - Daksh Shami, 2024.
+ [QuCT: A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) - Siwei Tan et al., MICRO, 2023
+ [Quantum Vulnerability Analysis to Guide Robust Quantum Computing System Design](https://arxiv.org/pdf/2207.14446) - Fang Qi et al., 2023
</br>


### 2. Middle-end Optimisations & Scheduling


#### Quantum Program Optimization #### 
+ [SuperstaQ: Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) - Campbell, Colin, et al. ,QCE, 2023
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/2109.03371) - Gushu Li, Anbang Wu, Yunong Shi, Ali Javadi-Abhari, Yufei Ding, Yuan Xie, 2021
+ [Enabling Dataflow Optimization for Quantum Programs](https://arxiv.org/abs/2101.11030) - David Ittah, Thomas Häner, Vadym Kliuchnikov, Torsten Hoefler, CoRR, 2021
+ [A Meet-in-the-Middle Algorithm for Fast Synthesis of Depth Optimal Quantum Circuits](https://arxiv.org/abs/1206.0758) - Matthew Amy, Dmitri Maslov, Michele Mosca, Martin Roetteler, IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems, 2021
+ [Automated optimization of large quantum circuits with continuous parameters](https://arxiv.org/abs/1710.07345) - Yunseong Nam, Neil J. Ross, Yuan Su, Andrew M. Childs, Dmitri Maslov, Nature npj Quantum Information, 2017
+ [A software methodology for compiling quantum programs](https://arxiv.org/abs/1604.01401) - Thomas Häner, Damian S. Steiger, Krysta Svore, Matthias Troyer,Quantum Science and Technology, 2016
+ [Exact synthesis of single-qubit unitaries over Clifford-cyclotomic gate sets](https://arxiv.org/abs/1501.04944) - Simon Forest, David Gosset, Vadym Kliuchnikov, David McKinnon, Journal of Mathematical Physics, 2015
+ [Polynomial-TimeT-Depth Optimization of Clifford+T Circuits Via Matroid Partitionin](https://arxiv.org/abs/1303.2042) - Matthew Amy, Dmitri Maslov, Michele Mosca, TCAD, 2013
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/abs/1810.00375) - Häner, Thomas, Hoefler, Torsten, Troyer, Matthias, OOPSLA, 2013
+ [Repeat-until-Success: Non-Deterministic Decomposition of Single-Qubit Unitaries](https://arxiv.org/abs/1311.1074) - Adam Paetznick, Krysta M. Svore, Quantum Information & Computation, 2013
+ [Circuit for Shor’s Algorithm Using 2n+3 Qubits](https://arxiv.org/abs/quant-ph/0205095) - Stephane Beauregard, Quantum Information and Computation, Quantum Information and Computation, 2002

#### Circuit Transformation ####
+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) - Francesco Preti,. Quantum, 2024
+ [Geyser: a compilation framework for quantum computing with neutral atoms](https://dl.acm.org/doi/abs/10.1145/3470496.3527428) - T. Patel et al., ISCA, 2022
+ [Backend compiler phases for trapped-ion quantum computers](https://arxiv.org/abs/2206.00544) - T. Schmale et al., 2022
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) - Fabian Kreppel et al., 2022

#### Qubit Mapping & Routing ####
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


### 3. Back-end & Hardware Execution / Runtime

#### Circuit Optimisation ####
+ [A Resource-Allocating Compiler for Lattice Surgery](https://arxiv.org/abs/2506.04620) - Alan Robertson, Haowen Gao, Yuval R. Sanders, 2025.
+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) - Francisco J. R. Ruiz, Nature Machine Intelligence, 2025.
+ [Q-Pilot: Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) - Hanrui Wang., DAC, 2024.
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) - Jonathan Durandau, Quantum, 2023.
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) - S.Ebadi et al., Science, 2022.
+ [Full-stack quantum computing systems in the NISQ era: algorithm-driven and hardware-aware compilation techniques](https://arxiv.org/abs/2204.06369) - Mendina Bandic, DATE, 2022.
+ [Software-hardware co-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - GushuLi, YunongShi, and AliJavadi-Abhari, ISCA, 2021.
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) - Zikun Li et al., OOPSLA, 2024
+ [Machine Learning Optimization of Quantum Circuit Layouts](https://dl.acm.org/doi/full/10.1145/3565271) - Alexandru Pale et al., ACM Transactions on Quantum Computing, 2023
+ [Synthesizing Quantum-Circuit Optimizers](https://dl.acm.org/doi/abs/10.1145/3591254) - Amanda Xu et al., PLDI, 2023 
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) - Bodo Rosenhahn, Tobias J. Osborne, 2023

#### Circuit Scheduling #### 
+ [Quantum circuit scheduler for QPUs usage optimization](https://arxiv.org/html/2404.01055v1) - Javier Romero-Alvarez et al. 2024
+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) - Toshinari Itoko, Takashi Imamichi, QCE, 2020
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) - Gian Giacomo Guerreschi, Jongsoo Park, Quantum Sci journal, 2017

#### Instruction Scheduling #### 
+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) - Philipp Seitz, Manuel Geiger, Christian Ufrecht, Axel Plinge, Christopher Mutschler, Daniel D. Scherer, Christian B. Mendl, Quantum Week, 2024
+ [DISQ: Dynamic Iteration Skipping for Variational Quantum Algorithms](https://arxiv.org/abs/2308.06634) - Junyao Zhang, Hanrui Wang, Gokul Subramanian Ravi, Frederic T. Chong, Song Han, Frank Mueller, Yiran Chen, QCE, 2023
+ [Let Each Quantum Bit Choose Its Basis Gates](https://arxiv.org/abs/2208.13380) - Sophia Fuhui Lin, Sara Sussman, Casey Duckering, Pranav S. Mundada, Jonathan M. Baker, Rohan S. Kumar, Andrew A. Houck, Frederic T. Chong, MICRO, 2022
+ [Software-hardwareco-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - Gushu Li, Yunong Shi, Ali Javadi-Abhari, ISCA 2021
+ [Error Mitigation in Quantum Computers through Instruction Scheduling](https://arxiv.org/abs/2105.01760) - Kaitlin N. Smith, Gokul Subramanian Ravi, Prakash Murali, Jonathan M. Baker, Nathan Earnest, Ali Javadi-Abhari, Frederic T. Chong, 2021
+ [EQC: ensembled quantum computing for variational quantum algorithms](https://arxiv.org/abs/2111.14940) - Samuel Stein, Yufei Ding, Nathan Wiebe, Bo Peng, Karol Kowalski, Nathan Baker, James Ang, Ang Li, ISCA, 2022
+ [Software mitigation of crosstalk on noisy intermediate-scale quantum computers](https://arxiv.org/abs/2001.02826) - Prakash Murali, David C. McKay, Margaret Martonosi, Ali Javadi-Abhari, ASPLOS, 2020
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/abs/2010.15876) - Xin-Chuan Wu, Dripto M. Debroy, Yongshan Ding, Jonathan M. Baker, Yuri Alexeev, Kenneth R. Brown, Frederic T. Chong, HPCA, 2020

#### Control level backend (Pulse scheduling, Optimal control, Fidelity optimisation, Pulse-level control, Hardware-aware compilation)

+ [Fast & Robust Gates via Hybrid Pulse Scheduling]
+ [A Time-Optimisation Framework Enabling Fast and Robust Gates in One Circuit](https://arxiv.org/pdf/2412.18533) - Eduardo Willwock Lussi et al., 2024.
+ [Short Two-Qubit Pulse Sequences for Exchange-Only Spin Qubits](https://arxiv.org/html/2412.14918v3) - Jason D. Chadwick et al., 2025.
+ [CCMap: Hardware-Aware Compilation for Chip-to-Chip Coupler-Connected QPUs](https://arxiv.org/abs/2505.09036) - Zefan Du, Shuwen Kan, Samuel Stein, Zhiding Liang, Ang Li, Ying Mao, 2025.
+ [QUAlibrate: Open-Source Framework that Cuts Calibration from Hours to Minutes]() - 2025.
+ [Qibolab: Pulse-Oriented Drivers for Custom Hardware](https://quantum-journal.org/papers/q-2024-02-12-1247/) - Stavros Efthymiou et al., Quantum, 2024.
+ [Sensitivity-Adapted Closed-Loop Optimisation for CZ Gates]()
+ [Pulse-Family Optimisation via Spectral Clustering](https://arxiv.org/abs/2408.00119) - Robert de Keijzer, Jurgen Snijders, André Carvalho, Servaas Kokkelmans, Quantum, 2024. 
+ [Architecting Noisy Intermediate-Scale Trapped Ion Quantum Computers](https://arxiv.org/abs/2004.04706) - Prakash Murali, Dripto M. Debroy, Kenneth R. Brown, and Margaret Martonosi, ISCA, 2020

#### Quantum ISA 
> "Bridging layer between Layout and Control"
+ [Design the Quantum Instruction Set with the Cartan Coordinate Analysis Framework](https://arxiv.org/abs/2410.04008) - Anbang Wu, Jingwen Leng, Minyi Guo, 2024.
+ [OpenQASM 3: A Broader and Deeper Quantum Assembly Language](https://dl.acm.org/doi/10.1145/3505636) - Andrew cross, et al., Transactions on Quantum Computing, 2022
+ [Open quantum assembly language](https://arxiv.org/abs/1707.03429) - Andrew W. Cross, Lev S. Bishop, John A. Smolin, Jay M. Gambetta, 2017
+ [A Practical Quantum Instruction Set Architecture](https://arxiv.org/abs/1608.03355) - Robert S. Smith, Michael J. Curtis, William J. Zeng, 2017
</br>


### 4. Verification & Benchmark / Simul & Debug 
#### Verification & Benchmark
+ [AutoQ 2.0: From Verification of Quantum Circuits to Verification of Quantum Programs](https://arxiv.org/abs/2411.09121) - Yu-Fang Chen, Kai-Min Chung, Min-Hsiu Hsieh, Wei-Jia Huang, Ondřej Lengál, Jyun-Ao Lin, Wei-Lun Tsai, TACAS, 2025.
+ [Verification of Quantum Circuits through Barrier Certificates using a Scenario Approach](https://arxiv.org/abs/2506.07635) - Siwei Hu, Victor Lopata, Sadegh Soudjani, Paolo Zuliani, QSW, 2025.
+ [MQT-QCEC v3.0](https://mqt.readthedocs.io/en/latest/)
#### Evaluation & Simulation 
+ [Benchmarking the performance of quantum computing software for quantum circuit creation, manipulation and compilation](https://www.nature.com/articles/s43588-025-00792-y) - Paul D. Nation, Abdullah Ash Saki, Sebastian Brandhofer, Luciano Bello, Shelly Garion, Matthew Treinish & Ali Javadi-Abhari, 2025
+ [QASMBench 1.4](https://github.com/pnnl/QASMBench) - TQC-2024.
+ [Azure QDK VS-Code Debugger](https://learn.microsoft.com/en-us/azure/quantum/testing-debugging) - 2024.
#### Debug & Test
+ [Cirq v1.4 simulators](https://quantumai.google/cirq/simulate/simulation)
+ [Qiskit SDK 0.50 primitives](https://docs.quantum.ibm.com/guides/simulate-with-qiskit-sdk-primitives)
+ [Bloq](https://arxiv.org/abs/2506.18458) - Noah H. Oldfield, Christoph Laaber, Shaukat Ali, 2025.
+ [MQT-Debugger framework](https://arxiv.org/abs/2412.12269) - Damian Rovara, Lukas Burgholzer, Robert Wille, 2024.
</br>


#### Error Mitigation and Correction 
> “Originally, it was part of the compiler stack, but because of the topic’s importance, I separated it"
+ [Resource-Efficient Context-Aware Dynamical Decoupling Embedding for Arbitrary Large-Scale Quantum Algorithms](https://link.aps.org/doi/10.1103/PRXQuantum.6.010332), Paul Coote et al., PRX Quantum, 2025
+ [Learning high-accuracy error decoding for quantum processors](https://www.nature.com/articles/s41586-024-08148-8) - Johannes Bausch et al., Nature, 2024
+ [Error Propagation-Aware Routing: A New Routing Strategy to Improve Success Rates of Quantum Circuits](https://dl.acm.org/doi/pdf/10.1145/3649476.3658790), Lu Fang et al., ICCAD, 2024 
+ [Learning How to Dynamically Decouple](https://arxiv.org/html/2405.08689v1), Arefur Rahman et al., arXiv, 2024.
+ [On the Use of Calibration Data in Error-Aware Compilation Techniques for NISQ Devices](https://arxiv.org/html/2407.21462v1), Handy Kurniawan et al., arXiv, 2024.
+ [TISCC: A Surface Code Compiler and Resource Estimator for Trapped-Ion Processors](https://dl.acm.org/doi/abs/10.1145/3624062.3624214) - Tyler Leblond, Ryan S. Bennink, Justin G. Lietz, and Christopher M. Seck, SC, 2023
 [Analyzing Strategies for Dynamical Decoupling Insertion on IBM Quantum](https://arxiv.org/abs/2204.14251), Murphy Y. Niu & Daniel A. Lidar, arXiv, 2022
+ [Qubit Mapping and Routing via MaxSAT](https://pages.cs.wisc.edu/~amolavi/files/micro22.pdf), Maryam Amiri et al., MICRO, 2022.
+ [VAQEM: A Variational Approach to Quantum Error Mitigation](https://www.computer.org/csdl/proceedings-article/hpca/2022/202700a288/1Ds0fvoYbCw), Gokul S. Ravi et al., HPCA, 2022
+ [Exploiting Long-Distance Interactions and Tolerating Atom Loss in Neutral Atom Quantum Architectures](https://arxiv.org/pdf/2111.06469.pdf) - Jonathan M. Baker, et al., ISCA, 2021
+ [ADAPT: Mitigating Idling Errors in Qubits via Adaptive Dynamical Decoupling](https://dl.acm.org/doi/10.1145/3466752.3480059), Poulami Das et al., MICRO, 2021
+ [A Noise-Aware Qubit Mapping Algorithm Evaluated via Qubit Interaction-Graph Criteria](https://www.researchgate.net/publication/350512755_A_Noise-Aware_Qubit_Mapping_Algorithm_Evaluated_via_Qubit_Interaction-Graph_Criteria), Matthew Steinberg et al., arXiv, 2021.
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) - Xin-Chuan Wu, Dripto M Debroy, Yongshan Ding, Jonathan M Baker, Yuri Alexeev, Kenneth R Brown, and Frederic T Chong, HPCA, 2020
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503), Yongshan Ding, Pranav Gokhale, Sophia Fuhui Lin, Richard Rines, Thomas Propson, Frederic T. Chong, MICRO, 2020
+ [Digital Zero-Noise Extrapolation for Quantum Error Mitigation](https://arxiv.org/abs/2005.10921), Tudor Giurgica-Tiron et al., IEEE QCE, 2020 
+ [Noise-Adaptive Compiler Mappings for NISQ Computers](https://dl.acm.org/doi/10.1145/3297858.3304075), Prakash Murali et al., ASPLOS, 2019
+ [Near-Optimal Routing of Noisy Quantum States](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/11134/111340A/Near-optimal-routing-of-noisy-quantum-states/10.1117/12.2526670.short), Kyle Cote et al., SPIE Proc., 2019.
+ [Not All Qubits Are Created Equal: Variation-Aware Qubit Allocation in NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007), Swamit Tannu & Moinuddin Qureshi, ASPLOS, 2019
+ [Practical Quantum Error Mitigation for Near-Future Applications](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509), Suguru Endo et al., Phys. Rev. X, 2018.  
+ [Error Mitigation for Short-Depth Quantum Circuits](https://link.aps.org/doi/10.1103/PhysRevLett.119.180509), Kristan Temme et al., Phys. Rev. Lett., 2017.

</br>




#### 🔬 Academic & Research Labs
+ [EPiQC Expedition](https://www.epiqc.cs.uchicago.edu/) - Research expedition on algorithm–hardware co-design and compiler stacks.  
+ [SIGPLAN Blog – “Verifying a Quantum Compiler”](https://blog.sigplan.org/2021/06/02/verifying-a-quantum-compiler/) - Deep dives into VOQC verified optimizations & proof techniques.  compiler/)  
+ [Quantum Frontiers – Caltech IQIM](https://quantumfrontiers.com/) - Essays on circuit depth, mapping, and quantum complexity.  
+ [QIR Alliance](https://www.qir-alliance.org/) - LLVM-based quantum IR spec & collaborative compiler tooling.   
+ [Azure Quantum QIR Docs](https://learn.microsoft.com/en-us/azure/quantum/concepts-qir) - Official semantic reference for QIR and related LLVM passes.    
+ [QIR Alliance GitHub](https://github.com/qir-alliance) - Open-source optimizers (QAT) and code-gen for QIR workflows.  
+ [OpenQASM 3 MLIR Compiler – qe-compiler](https://github.com/openqasm/qe-compiler) - MLIR dialect pipeline targeting OpenQASM 3 and NISQ devices. 
+ [Pandora – Aalto University](https://aaltodoc.aalto.fi/items/1d6b3201-b181-4a55-9eec-0e23119b1b38) - Million-gate optimization & equivalence-checking toolkit.   
+ [Giallar Verification Toolkit](https://arxiv.org/abs/2205.00661) - Push-button semantic-preservation proofs for Qiskit passes.   
+ [Composable Quantum Compiler – POPL’21 Paper](https://rand.cs.uchicago.edu/files/popl_2021_slides.pdf) - Coq-based SQIR/VOQC compositional compiler design.

#### 💻 Tech-Giants & Start-ups
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

#### 📚 Books
+ [Quantum Computer Systems: Research for Noisy Intermediate-Scale Quantum Computers](https://www.amazon.co.uk/Quantum-Computer-Synthesis-Lectures-Architecture/dp/168173866X) – NISQ-era architecture/​compiler co-design guide.  
+ [Quantum Computing for Computer Architects, 2e](https://link.springer.com/book/10.1007/978-3-031-01731-5) – ISA design, cost models and hardware-aware optimisation.  
+ [Programming Quantum Computers](https://www.oreilly.com/library/view/programming-quantum-computers/9781492039673/) – Hands-on circuit building, transpilation & benchmarking across Qiskit, Q# and PyQuil.  
+ [Quantum Computing: An Applied Approach, 2e](https://link.springer.com/book/10.1007/978-3-030-83274-2) – Tutorials on mapping, error mitigation and full-stack workflows.  
+ [Quantum Software Engineering](https://link.springer.com/book/10.1007/978-3-031-05324-5) – Methods, metrics and tooling for the quantum-software life-cycle.  
+ [Quantum Software: Aspects of Theory and System Design](https://link.springer.com/book/10.1007/978-3-031-64136-7) – Hardware-agnostic survey of optimisation and deployment patterns.  
+ [Building Quantum Software with Python](https://www.manning.com/books/building-quantum-software-with-python) – Developer-centric guide to writing and transpiling circuits in Python.  
+ [Software Engineering for Quantum Computing](https://www.amazon.ca/Software-Engineering-Quantum-Computing-Publishing/dp/1446184668) – Design patterns, CI/CD and project workflows for NISQ projects.  


#### 🗓️ Conferences & Symposia
+ [HPCA – IEEE Int’l Symp. on High-Performance Computer Architecture](https://hpca-conf.org/) – Architecture-level optimisations, including quantum/classical co-design.  
+ [ASPLOS – Architectural Support for Programming Languages & Operating Systems](https://www.asplos-conference.org/) – Cross-layer hardware/software studies.  
+ [ISCA – Int’l Symp. on Computer Architecture](https://iscaconf.org/) – Next-gen processor and compiler interactions.  
+ [MICRO – IEEE/ACM Int’l Symp. on Microarchitecture](https://www.microarch.org/) – Micro-architectural support for quantum accelerators.  
+ [ICCAD – IEEE/ACM Int’l Conf. on CAD](https://iccad.com/) – EDA techniques and synthesis for quantum circuits.  
+ [DAC – Design Automation Conference](https://www.dac.com/) – Tool flows, verification and design-automation research.  
+ [CC – Int’l Conf. on Compiler Construction](https://conf.researchr.org/series/cc) – Classic compiler theory now extending to quantum IRs.  
+ [PLDI – Programming Language Design & Implementation](https://conf.researchr.org/series/pldi) – Language semantics and optimisation passes.  
+ [QCE – IEEE Quantum Week](https://qce.quantum.ieee.org/) – End-to-end quantum-computing stack with dedicated compiler tracks.  
+ [CF – ACM Computing Frontiers](https://www.computingfrontiers.org/) – Emerging architectures, including quantum hardware/software.  
+ [IEEE QSW – Int’l Conf. on Quantum Software](https://services.conferences.computer.org/2025/qsw/) – Quantum-software engineering, verification and toolchains.  
+ [IQSOFT – Int’l Conf. on Quantum Software](https://iqsoft.scitevents.org/) – Six-track event focused on optimisation, runtime and testing.  
+ [QIP – Quantum Information Processing](https://qipconference.org/) – Theory sessions on depth/T-count lower bounds and circuit optimisation.  
+ [TQC – Theory of Quantum Computation, Communication & Cryptography](https://tqc-conference.org/) – Foundational results feeding compiler theory.  
+ [QPL – Quantum Physics & Logic](https://qpl2025.github.io/) – Type systems, categorical semantics and verifiable quantum languages.  


#### 📰 Journals
+ [IEEE Transactions on Quantum Engineering](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=8780379) – Hardware-aware compilation and systems papers.  
+ [Quantum Information & Computation](http://www.rintonpress.com/journals/qic.html) – Algorithms, complexity and optimisation studies.  
+ [Quantum Science and Technology](https://iopscience.iop.org/journal/2058-9565) – Experimental and theoretical advances, incl. compiler tooling.  
+ [Proceedings of the ACM on Programming Languages / PACMPL](https://dl.acm.org/journal/pacmpl) – PLDI & OOPSLA issues often feature quantum-language work.  
+ [Journal of Mathematical Physics](https://aip.scitation.org/journal/jmp) – Formal techniques underlying verification and synthesis.  
+ [IEEE Transactions on CAD of Integrated Circuits & Systems](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=43) – Placement, routing and design-automation for quantum chips.  
+ [ACM Transactions on Quantum Computing](https://dl.acm.org/journal/tqc) – Dedicated venue for compiler, runtime and architecture papers.  
+ [Computing Research Repository (CoRR)](https://arxiv.org/corr) – Pre-prints; quickest way to track new transpilation work.  
+ [npj Quantum Information)[https://www.nature.com/npjqi) – Nature-branded, high-impact quantum-software and algorithms.  
+ [PRX Quantum](https://journals.aps.org/prxquantum) – APS open-access journal for architecture and optimisation breakthroughs.  
+ [Quantum](https://quantum-journal.org/)– Overlay journal; steady flow of compiler and language articles.  
+ [Quantum Engineering](https://onlinelibrary.wiley.com/journal/26395307) – Engineering-oriented studies of full-stack toolchains.  
+ [Quantum Machine Intelligence](https://link.springer.com/journal/42484) – ML-driven layout, scheduling and heuristic optimisation.  
+ [Advanced Quantum Technologies](https://onlinelibrary.wiley.com/journal/2511902X) – Experimental control-level compilation and pulse studies.  
+ [Nature](https://www.nature.com/) – Occasional landmark papers on scalable compilation and error correction.  
+ [Nature Physics](https://www.nature.com/nphys) – Hardware/​software co-design breakthroughs.  
+ [Nature Communications](https://www.nature.com/ncomms) – Open-access venue for interdisciplinary quantum-compiler work.  
+ [OOPSLA – Proc. of the ACM on Programming Languages, OOPSLA issue](https://conf.researchr.org/series/oopsla) – Object-oriented languages & optimisation; now features quantum PL papers.  



# Awesome-Quantum-Compilers
This repository focuses on the research and study of quantum compilers. It aims to explore the translation of high-level quantum programming languages into low-level instructions executable on quantum hardware.

The workflow of quantum compilation is categorized into six major stages, providing a broad structural overview. Additionally, the repository includes concepts such as Verification and Evaluation and Simulation and Testing.

There are also plans to tag each paper with keywords according to the target quantum architecture.


+ Research Papers
  + Quantum Compilation Surveys
  + Front-end IR / High-Level Representation
  + Quantum Program Optimization
  + Quantum IR
  + Circuit Transformation 
  + Routing and Mapping 
  + Optimization and Scheduling
  + Quantum Circuit Optimisation
  + Quantum Circuit Scheduling
  + Quantum Instruction Scheduling
  + Quantum Circuit Analysis
  + Error Mitigation and Correction
  + Hardware Execution & Runtime Scheduler 
  + Verification 
  + Benchmarking / Evaluation
  + Simulation + Debug/Test
+ Books
+ Related-Repo & Post
+ Benchmarks and Datasets
+ Conferences
+ Journals





### Research Papers

#### Quantum Compilation Surveys
+ [Quantum Compilation Process: A Survey](https://link.springer.com/chapter/10.1007/978-3-031-90200-0_9) - F. Javier Cardama, Jorge Vázquez-Pérez, Tomás F. Pena, Juan C. Pichel & Andrés Gómez, 2025
+ [Quantum Compiler Design for Qubit Mapping and Routing](https://arxiv.org/pdf/2505.16891) - Chenghong zhu et al., 2025.
+ [A Comprehensive Review of Quantum Circuit Optimization: Current Trends and Future Directions](https://www.mdpi.com/2624-960X/7/1/2) - Krishnageetha Karuppasamy et al., 2025.
+ [Quantum Circuit Synthesis and Compilation Optimization: Overview and Prospects](https://arxiv.org/html/2407.00736v1) - Ge Yan et al., 2024.
+ [Quantum Compiling](https://arxiv.org/abs/2112.00187) - Marco Maronese, Lorenzo Moro, Lorenzo Rocutto, Enrico Prati, 2021
+ [Quantum compiling by deep reinforcement learning](https://www.nature.com/articles/s42005-021-00684-3) - Lorenzo Moro, Matteo G. A. Paris, Marcello Restelli, Enrico Prati, Nature, 2021
+ [Programming languages and compiler design for realistic quantum hardware](https://www.nature.com/articles/nature23459) - Frederic T. Chong, Diana Franklin, Margaret Martonosi, Nature, 2017



</br></br>
#### Front-end IR / High-Level Representation ####
#### QASM, High-level synthesis, IR Design, Program synthesis, High-level abstraction, Loop optimization, Program transformation
+ [LinguaQuanta: Towards a Quantum Transpiler Between OpenQASM and Quipper](https://arxiv.org/pdf/2404.08147) - Scott Wesley, 2024.
+ [Design and synthesis of scalable quantum programs](https://arxiv.org/abs/2412.07372) - Tomer Goldfriend et al., 2025.
+ [PHOENIX: Pauli-Based High-Level Optimization Engine for Instruction Execution on NISQ Devices](https://arxiv.org/abs/2504.03529) - Zhaohui Yang et al.,2025.
+ [Practical and efficient quantum circuit synthesis and transpiling with Reinforcement Learning](https://arxiv.org/abs/2405.13196) - David Kremer et al.,2025.
+ [Qmod: Expressive High-Level Quantum Modeling]([Matan Vax](https://arxiv.org/html/2502.19368v1) - Matan Vax et al., 2025. 
####  Quantum Program Representation #### 
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) - David Ittah, Thomas Häner, Vadym Kliuchnikov, Torsten Hoefler, ACM Transactions on Quantum Computing, 2021.
  
####  Quantum Program Optimization #### 
+ [SuperstaQ: Deep Optimization of Quantum Program](https://arxiv.org/abs/2309.05157) - Campbell, Colin, et al. ,QCE, 2023
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/2109.03371) - Gushu Li, Anbang Wu, Yunong Shi, Ali Javadi-Abhari, Yufei Ding, Yuan Xie, 2021
+ [Enabling Dataflow Optimization for Quantum Programs](https://arxiv.org/abs/2101.11030) - David Ittah, Thomas Häner, Vadym Kliuchnikov, Torsten Hoefler, CoRR, 2021
+ [A Meet-in-the-Middle Algorithm for Fast Synthesis of Depth Optimal Quantum Circuits](https://arxiv.org/abs/1206.0758) - Matthew Amy, Dmitri Maslov, Michele Mosca, Martin Roetteler, IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems, 2021
+ [Automated optimization of large quantum circuits with continuous parameters](https://arxiv.org/abs/1710.07345) - Yunseong Nam, Neil J. Ross, Yuan Su, Andrew M. Childs, Dmitri Maslov, Nature npj Quantum Information, 2017
+ [A software methodology for compiling quantum programs](https://arxiv.org/abs/1604.01401) - Thomas Häner, Damian S. Steiger, Krysta Svore, Matthias Troyer, 
Quantum Science and Technology, 2016
+ [Exact synthesis of single-qubit unitaries over Clifford-cyclotomic gate sets](https://arxiv.org/abs/1501.04944) - Simon Forest, David Gosset, Vadym Kliuchnikov, David McKinnon, Journal of Mathematical Physics, 2015
+ [Polynomial-TimeT-Depth Optimization of Clifford+T Circuits Via Matroid Partitionin](https://arxiv.org/abs/1303.2042) - Matthew Amy, Dmitri Maslov, Michele Mosca, TCAD, 2013
+ [Assertion-Based Optimization of Quantum Programs](https://arxiv.org/abs/1810.00375) - Häner, Thomas, Hoefler, Torsten, Troyer, Matthias, OOPSLA, 2013
+ [Repeat-until-Success: Non-Deterministic Decomposition of Single-Qubit Unitaries](https://arxiv.org/abs/1311.1074) - Adam Paetznick, Krysta M. Svore, Quantum Information & Computation, 2013
+ [Circuit for Shor’s Algorithm Using 2n+3 Qubits](https://arxiv.org/abs/quant-ph/0205095) - Stephane Beauregard, Quantum Information and Computation, Quantum Information and Computation, 2002
  
#### Quantum IR #### 
+ [A Cross-Platform Execution Engine for the Quantum Intermediate Representation](https://arxiv.org/pdf/2404.14299) - Elaine Wong et al., 2024
+ [InQuIR: Intermediate Representation for Interconnected Quantum Computers](https://arxiv.org/abs/2302.00267) - Shin Nishio, Ryo Wakizaka, 2023
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) - Anurudh Peduri, Siddharth Bhat, CC, 2022
+ [Quantum circuit transformations with a multi-level intermediate representation compiler](https://arxiv.org/abs/2112.10677) - T. Nguyen et al., 2021
+ [Enabling Retargetable Optimizing Compilers for Quantum Accelerators via a Multi-Level Intermediate Representation](https://arxiv.org/abs/2109.00506) - Thien Nguyen, Alexander McCaskey, 2021
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) - Alexander McCaskey, Thien Nguyen, QCE, 2021
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) - Ali JavadiAbhari, Shruti Patil, Daniel Kudrow, Jeff Heckey, Alexey Lvov, Frederic T. Chong, Margaret Martonosi, Parallel Comput, CF, 2014
+ [Introducing Quantum Intermediate Representation (QIR)](https://devblogs.microsoft.com/qsharp/introducing-quantum-intermediate-representation-qir/)



</br></br>
#### Circuit Transformation ####
#### Gate Synthesis, Gate Decomposition, Basis Gates

+ [Hybrid discrete-continuous compilation of trapped-ion quantum circuits with deep reinforcement learning](https://arxiv.org/abs/2307.05744) - Francesco Preti,. Quantum, 2024
+ [Geyser: a compilation framework for quantum computing with neutral atoms](https://dl.acm.org/doi/abs/10.1145/3470496.3527428) - T. Patel et al., ISCA, 2022
+ [Backend compiler phases for trapped-ion quantum computers](https://arxiv.org/abs/2206.00544) - T. Schmale et al., 2022
+ [Quantum Circuit Compiler for a Shuttling-Based Trapped Ion Quantum Computer](https://arxiv.org/pdf/2207.01964v2.pdf) - Fabian Kreppel et al., 2022
</br></br>


#### SWAP optimization, Connectivity constraints, Circuit Partitioning
#### Qubit Routing and Mapping #### 
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



</br></br>
#### Optimisation and Scheduling 
#### Circuit Depth Reduction, Gate Scheduling, Resource estimation, Circuit Scheduling, Circuit Optimization

+ [Quantum circuit optimization with AlphaTensor](https://www.nature.com/articles/s42256-025-01001-1) - Francisco J. R. Ruiz, Nature Machine Intelligence, 2025
+ [Q-Pilot: Field Programmable Qubit Array Compilation with Flying Ancillas](https://arxiv.org/abs/2311.16190) - Hanrui Wang., DAC, 2024
+ [Automated Generation of Shuttling Sequences for a Linear Segmented Ion Trap Quantum Computer](https://arxiv.org/abs/2208.04881) - Jonathan Durandau, Quantum, 2023
+ [Quantum optimization of maximum independent set using Rydberg atom arrays](https://arxiv.org/abs/2202.09372) - S.Ebadi et al., Science, 2022
+ [Full-stack quantum computing systems in the NISQ era: algorithm-driven and hardware-aware compilation techniques](https://arxiv.org/abs/2204.06369) - Mendina Bandic, DATE, 2022
+ [Software-hardware co-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - GushuLi, YunongShi, and AliJavadi-Abhari, ISCA, 2021

#### Quantum Circuit Optimisation #### 
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) - Zikun Li et al., OOPSLA, 2024
+ [Machine Learning Optimization of Quantum Circuit Layouts](https://dl.acm.org/doi/full/10.1145/3565271) - Alexandru Pale et al., ACM Transactions on Quantum Computing, 2023
+ [Synthesizing Quantum-Circuit Optimizers](https://dl.acm.org/doi/abs/10.1145/3591254) - Amanda Xu et al., PLDI, 2023 
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) - Bodo Rosenhahn, Tobias J. Osborne, 2023

#### Quantum Circuit Scheduling #### 
+ [Quantum circuit scheduler for QPUs usage optimization](https://arxiv.org/html/2404.01055v1) - Javier Romero-Alvarez et al. 2024
+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) - Toshinari Itoko, Takashi Imamichi, QCE, 2020
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) - Gian Giacomo Guerreschi, Jongsoo Park, Quantum Sci journal, 2017

#### Quantum Instruction Scheduling #### 
+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) - Philipp Seitz, Manuel Geiger, Christian Ufrecht, Axel Plinge, Christopher Mutschler, Daniel D. Scherer, Christian B. Mendl, Quantum Week, 2024
+ [DISQ: Dynamic Iteration Skipping for Variational Quantum Algorithms](https://arxiv.org/abs/2308.06634) - Junyao Zhang, Hanrui Wang, Gokul Subramanian Ravi, Frederic T. Chong, Song Han, Frank Mueller, Yiran Chen, QCE, 2023
+ [Let Each Quantum Bit Choose Its Basis Gates](https://arxiv.org/abs/2208.13380) - Sophia Fuhui Lin, Sara Sussman, Casey Duckering, Pranav S. Mundada, Jonathan M. Baker, Rohan S. Kumar, Andrew A. Houck, Frederic T. Chong, MICRO, 2022
+ [Software-hardwareco-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - Gushu Li, Yunong Shi, Ali Javadi-Abhari, ISCA 2021
+ [Error Mitigation in Quantum Computers through Instruction Scheduling](https://arxiv.org/abs/2105.01760) - Kaitlin N. Smith, Gokul Subramanian Ravi, Prakash Murali, Jonathan M. Baker, Nathan Earnest, Ali Javadi-Abhari, Frederic T. Chong, 2021
+ [EQC: ensembled quantum computing for variational quantum algorithms](https://arxiv.org/abs/2111.14940) - Samuel Stein, Yufei Ding, Nathan Wiebe, Bo Peng, Karol Kowalski, Nathan Baker, James Ang, Ang Li, ISCA, 2022
+ [Software mitigation of crosstalk on noisy intermediate-scale quantum computers](https://arxiv.org/abs/2001.02826) - Prakash Murali, David C. McKay, Margaret Martonosi, Ali Javadi-Abhari, ASPLOS, 2020
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/abs/2010.15876) - Xin-Chuan Wu, Dripto M. Debroy, Yongshan Ding, Jonathan M. Baker, Yuri Alexeev, Kenneth R. Brown, Frederic T. Chong, HPCA, 2020

#### Quantum Circuit Analysis #### 
+ [Character Complexity: A Novel Measure for Quantum Circuit Analysis](https://arxiv.org/abs/2408.09641) - Daksh Shami, 2024.
+ [QuCT: A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) - Siwei Tan et al., MICRO, 2023
+ [Quantum Vulnerability Analysis to Guide Robust Quantum Computing System Design](https://arxiv.org/pdf/2207.14446) - Fang Qi et al., 2023
</br></br>


#### Error Mitigation and Correction ####

+ [Learning high-accuracy error decoding for quantum processors](https://www.nature.com/articles/s41586-024-08148-8) - Johannes Bausch et al, Nature, 2024
+ [TISCC: A Surface Code Compiler and Resource Estimator for Trapped-Ion Processors](https://dl.acm.org/doi/abs/10.1145/3624062.3624214) - Tyler Leblond, Ryan S. Bennink, Justin G. Lietz, and Christopher M. Seck, SC, 2023
+ [Exploiting Long-Distance Interactions and Tolerating Atom Loss in Neutral Atom Quantum Architectures](https://arxiv.org/pdf/2111.06469.pdf) -  Jonathan M. Baker, et al. ISCA, 2021
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/pdf/2010.15876v3.pdf) - Xin-Chuan Wu, Dripto M Debroy, Yongshan Ding, Jonathan M Baker, Yuri Alexeev, Kenneth R Brown, and Frederic T Chong, HPCA, 2020
+ [Systematic Cross talk Mitigation for Superconducting Qubits via Frequency-Aware Compilation](https://arxiv.org/abs/2008.09503), Yongshan Ding, Pranav Gokhale, Sophia Fuhui Lin, Richard Rines, Thomas Propson, Frederic T. Chong, MICRO, 2020
</br></br>

#### Noise-Aware Compilation ####

#### Hardware Execution & Runtime Scheduler 
#### Pulse scheduling, Optimal control, Fidelity optimization, Pulse-Level Control, Hardware-aware compilation

+ [Architecting Noisy Intermediate-Scale Trapped Ion Quantum Computers](https://arxiv.org/abs/2004.04706) - Prakash Murali, Dripto M. Debroy, Kenneth R. Brown, and Margaret Martonosi, ISCA, 2020

#### Quantum ISA #### 
+ [OpenQASM 3: A Broader and Deeper Quantum Assembly Language](https://dl.acm.org/doi/10.1145/3505636) - Andrew cross, et al., Transactions on Quantum Computing, 2022
+ [Open quantum assembly language](https://arxiv.org/abs/1707.03429) - Andrew W. Cross, Lev S. Bishop, John A. Smolin, Jay M. Gambetta, 2017
+ [A Practical Quantum Instruction Set Architecture](https://arxiv.org/abs/1608.03355) - Robert S. Smith, Michael J. Curtis, William J. Zeng, 2017


</br></br>
#### Verification ####
+ [AutoQ 2.0: From Verification of Quantum Circuits to Verification of Quantum Programs](https://arxiv.org/abs/2411.09121) - Yu-Fang Chen, Kai-Min Chung, Min-Hsiu Hsieh, Wei-Jia Huang, Ondřej Lengál, Jyun-Ao Lin, Wei-Lun Tsai, TACAS, 2025.
+ [Verification of Quantum Circuits through Barrier Certificates using a Scenario Approach](https://arxiv.org/abs/2506.07635) - Siwei Hu, Victor Lopata, Sadegh Soudjani, Paolo Zuliani, QSW, 2025.
+ [MQT-QCEC v3.0](https://mqt.readthedocs.io/en/latest/)


#### Benchmarking / Evaluation ####
+ [Benchmarking the performance of quantum computing software for quantum circuit creation, manipulation and compilation](https://www.nature.com/articles/s43588-025-00792-y) - Paul D. Nation, Abdullah Ash Saki, Sebastian Brandhofer, Luciano Bello, Shelly Garion, Matthew Treinish & Ali Javadi-Abhari, 2025
+ [QASMBench 1.4](https://github.com/pnnl/QASMBench) - TQC-2024.
+ [Azure QDK VS-Code Debugger](https://learn.microsoft.com/en-us/azure/quantum/testing-debugging) - 2024.
</br></br>


#### Simulation + Debug/Test ####
+ [Cirq v1.4 simulators](https://quantumai.google/cirq/simulate/simulation)
+ [Qiskit SDK 0.50 primitives](https://docs.quantum.ibm.com/guides/simulate-with-qiskit-sdk-primitives)
+ [Bloq](https://arxiv.org/abs/2506.18458) - Noah H. Oldfield, Christoph Laaber, Shaukat Ali, 2025.
+ [MQT-Debugger framework](https://arxiv.org/abs/2412.12269) - Damian Rovara, Lukas Burgholzer, Robert Wille, 2024.
</br></br>



#### Books ####
+ [Quantum Computer Systems: Research for Noisy Intermediate-Scale Quantum Computers](https://www.amazon.co.uk/Quantum-Computer-Synthesis-Lectures-Architecture/dp/168173866X) Yongshan ding, 2020
+ [Quantum Computing for Computer Architects, Second Edition](https://link.springer.com/book/10.1007/978-3-031-01731-5] - Tzvetan S. Metodi , Arvin I. Faruque , Frederic T. Chong, 2011.


#### Learning Resources and Blogs ####
+ [Qauntum Computing Systems - Yufei ding](https://cseweb.ucsd.edu/~yufeiding/CSE291QC/)
+ [Quantum Computing - Luca Trevisan](https://cs.stanford.edu/people/trevisan/quantum/)
+ [QuTech Academic](https://www.qutube.nl/)
+ [The Quantum Insider](https://thequantuminsider.com/) 
+ [Google Quantum AI](https://quantumai.google/)
+ [IBM Quantum Blog](https://www.ibm.com/quantum/blog)
+ [Nvidia Quantum Computing](https://developer.nvidia.com/blog/tag/quantum-computing/)
+ [Quantinuum Blog](https://www.quantinuum.com/news/blog)

  
#### Conference
 + HPCA, ASPLOS, ISCA, MICRO, ICCAD, DAC, CC, PLDI </br>
 + QCE(Quantum Computing and Engineering) </br>
 + CF(Computing Frontiers)

#### Journal
 + IEEE Transactions on Quantum Engineering </br>
 + Quantum Information & Computation </br>
 + Quantum Science and Technology </br>
 + ACM on Programming Languages </br>
 + Journal of Mathematical Physic </br>
 + Quantum Information and Computation </br>
 + IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems </br>
 + ACM Transactions on Quantum Computing </br>
 + Computing Research Repository(CoRR) </br>
 + Nature npj Quantum Information </br>
 + Transactions on Computer-Aided Design of Integrated Circuits and Systems </br>
 + OOPSLA



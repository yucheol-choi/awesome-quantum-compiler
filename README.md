# Awesome-Quantum-Compilers
This repository focuses on the research and study of quantum compilers. It aims to explore the translation of high-level quantum programming languages into low-level instructions executable on quantum hardware.

The workflow of quantum compilation is categorized into six major stages, providing a broad structural overview. Additionally, the repository includes concepts such as Verification and Evaluation and Simulation and Testing.

There are also plans to tag each paper with keywords according to the target quantum architecture.


+ paper
  + General Quantum Compiler
  + High-Level Representation 
  + Circuit Transformation 
  + Routing and Mapping 
  + Optimization and Scheduling 
  + Error Mitigation and Correction 
  + Hardware Execution
  + Verification and Evaluation
  + Simulation and Testing
+ Books
+ Related-Repo & Post
+ Benchmarks and Datasets
+ Conferences
+ Journals





# Papers

## General Research
+ [Quantum Compiling](https://arxiv.org/abs/2112.00187) - Marco Maronese, Lorenzo Moro, Lorenzo Rocutto, Enrico Prati, 2021
+ [Quantum compiling by deep reinforcement learning](https://www.nature.com/articles/s42005-021-00684-3) - Lorenzo Moro, Matteo G. A. Paris, Marcello Restelli, Enrico Prati, Nature, 2021
+ [Programming languages and compiler design for realistic quantum hardware](https://www.nature.com/articles/nature23459) - Frederic T. Chong, Diana Franklin, Margaret Martonosi, Nature, 2017



</br></br>
## 1. High-Level Representation (Program Optimization, Program Representation, Intermediate Representation)
**Keywords** : QASM, High-level synthesis, IR Design, Program synthesis, High-level abstraction, Loop optimization, Program transformation

### 🔹 Quantum Program Representation 🔹 ### 
+ [QIRO: A Static Single Assignment-based Quantum Program Representation for Optimization](https://dl.acm.org/doi/10.1145/3491247) - David Ittah, Thomas Häner, Vadym Kliuchnikov, Torsten Hoefler, ACM Transactions on Quantum Computing, 2021 
### 🔹 Quantum Program Optimization 🔹 ### 
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
### 🔹 Quantum IR 🔹 ### 
+ [A Cross-Platform Execution Engine for the Quantum Intermediate Representation](https://arxiv.org/pdf/2404.14299) - Elaine Wong et al., 2024
+ [InQuIR: Intermediate Representation for Interconnected Quantum Computers](https://arxiv.org/abs/2302.00267) - Shin Nishio, Ryo Wakizaka, 2023
+ [QSSA: an SSA-based IR for Quantum computing](https://arxiv.org/abs/2109.02409) - Anurudh Peduri, Siddharth Bhat, CC, 2022
+ [Quantum circuit transformations with a multi-level intermediate representation compiler](https://arxiv.org/abs/2112.10677) - T. Nguyen et al., 2021
+ [Enabling Retargetable Optimizing Compilers for Quantum Accelerators via a Multi-Level Intermediate Representation](https://arxiv.org/abs/2109.00506) - Thien Nguyen, Alexander McCaskey, 2021
+ [A MLIR Dialect for Quantum Assembly Languages](https://arxiv.org/abs/2101.11365) - Alexander McCaskey, Thien Nguyen, QCE, 2021
+ [ScaffCC: A Framework for Compilation and Analysis of Quantum Computing Programs](https://arxiv.org/abs/1507.01902) - Ali JavadiAbhari, Shruti Patil, Daniel Kudrow, Jeff Heckey, Alexey Lvov, Frederic T. Chong, Margaret Martonosi, Parallel Comput, CF, 2014
+ [Introducing Quantum Intermediate Representation (QIR)](https://devblogs.microsoft.com/qsharp/introducing-quantum-intermediate-representation-qir/)



</br></br>
## 2. Circuit Transformation (Gate Decomposition, Basis gate conversion)
**Keywords** : Gate synthesis, Gate decomposition, Basis gates



</br></br>
## 3. Routing and Mapping (Qubit Mapping, Routing, Circuit Partitioning)
**Keywords** : Qubit mapping, SWAP optimization, Connectivity constraints
### 🔹 Qubit Mapping 🔹 ### 
+ [Qubit Mapping Toward Quantum Advantage](https://arxiv.org/pdf/2210.01306v1.pdf) - Chin-Yi Cheng et al., 2022
+ [Qubit Mapping and Routing via MaxSAT](https://arxiv.org/abs/2208.13679v1) - Abtin Molavi, Amanda Xu, Martin Diges, Lauren Pick, Swamit Tannu, Aws Albarghouthi, MICRO, 2022
+ [Paulihedral: a generalized block-wise compiler optimization framework for Quantum simulation kernels](https://arxiv.org/abs/1901.11054) - Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi, ASPLOS, 19
+ [QuCloud: A New Qubit Mapping Mechanism for Multi-programming Quantum Computing in Cloud Environment](https://ieeexplore.ieee.org/document/9407180) - Lei Liu, Xinglei Dou, HPCA, 2021
+ [Time-optimal Qubit mapping](https://dl.acm.org/doi/pdf/10.1145/3445814.3446706) - Chi Zhang et al., ASPLOS, 2021
+ [Not All Qubits Are Created Equal: A Case for Variability-Aware Policies for NISQ-Era Quantum Computers](https://dl.acm.org/doi/10.1145/3297858.3304007) - Swamit S. Tannu, Moinuddin K. Qureshi, ASPLOS, 2019
+ [Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.](https://arxiv.org/abs/1901.11054) - Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi, ASPLOS, 2019



</br></br>
## 4. Optimization and Scheduling (Circuit Scheduling Instruction Scheduling, Circuit Optimization, Resource Estimation, Circuit Analysis)
**Keywords** : Circuit depth reduction, Parallel execution, Gate scheduling, Resource estimation
### 🔹 Quantum Circuit Optimization 🔹 ### 
+ [Quarl: A Learning-Based Quantum Circuit Optimizer](https://dl.acm.org/doi/abs/10.1145/3649831) - Zikun Li et al., OOPSLA, 2024
+ [Machine Learning Optimization of Quantum Circuit Layouts](https://dl.acm.org/doi/full/10.1145/3565271) - Alexandru Pale et al., ACM Transactions on Quantum Computing, 2023
+ [Synthesizing Quantum-Circuit Optimizers](https://dl.acm.org/doi/abs/10.1145/3591254) - Amanda Xu et al., PLDI, 2023 
+ [Monte Carlo Graph Search for Quantum Circuit Optimization](https://arxiv.org/abs/2307.07353) - Bodo Rosenhahn, Tobias J. Osborne, 2023
### 🔹 Quantum Circuit Scheduling 🔹 ### 
+ [Quantum circuit scheduler for QPUs usage optimization](https://arxiv.org/html/2404.01055v1) - Javier Romero-Alvarez et al. 2024
+ [Scheduling of Operations in Quantum Compiler](https://arxiv.org/pdf/2011.04936) - Toshinari Itoko, Takashi Imamichi, QCE, 2020
+ [Two-step approach to scheduling quantum circuits](https://arxiv.org/abs/1708.00023) - Gian Giacomo Guerreschi, Jongsoo Park, Quantum Sci journal, 2017
### 🔹 Quantum Instruction Scheduling 🔹 ### 
+ [SCIM MILQ: An HPC Quantum Scheduler](https://arxiv.org/abs/2404.03512) - Philipp Seitz, Manuel Geiger, Christian Ufrecht, Axel Plinge, Christopher Mutschler, Daniel D. Scherer, Christian B. Mendl, Quantum Week, 2024
+ [DISQ: Dynamic Iteration Skipping for Variational Quantum Algorithms](https://arxiv.org/abs/2308.06634) - Junyao Zhang, Hanrui Wang, Gokul Subramanian Ravi, Frederic T. Chong, Song Han, Frank Mueller, Yiran Chen, QCE, 2023
+ [Let Each Quantum Bit Choose Its Basis Gates](https://arxiv.org/abs/2208.13380) - Sophia Fuhui Lin, Sara Sussman, Casey Duckering, Pranav S. Mundada, Jonathan M. Baker, Rohan S. Kumar, Andrew A. Houck, Frederic T. Chong, MICRO, 2022
+ [Software-hardwareco-optimization for computational chemistry on superconducting quantum processors](https://arxiv.org/abs/2105.07127) - Gushu Li, Yunong Shi, Ali Javadi-Abhari, ISCA 2021
+ [Error Mitigation in Quantum Computers through Instruction Scheduling](https://arxiv.org/abs/2105.01760) - Kaitlin N. Smith, Gokul Subramanian Ravi, Prakash Murali, Jonathan M. Baker, Nathan Earnest, Ali Javadi-Abhari, Frederic T. Chong, 2021
+ [EQC: ensembled quantum computing for variational quantum algorithms](https://arxiv.org/abs/2111.14940) - Samuel Stein, Yufei Ding, Nathan Wiebe, Bo Peng, Karol Kowalski, Nathan Baker, James Ang, Ang Li, ISCA, 2022
+ [Software mitigation of crosstalk on noisy intermediate-scale quantum computers](https://arxiv.org/abs/2001.02826) - Prakash Murali, David C. McKay, Margaret Martonosi, Ali Javadi-Abhari, ASPLOS, 2020
+ [TILT: Achieving Higher Fidelity on a Trapped-Ion Linear-Tape Quantum Computing Architecture](https://arxiv.org/abs/2010.15876) - Xin-Chuan Wu, Dripto M. Debroy, Yongshan Ding, Jonathan M. Baker, Yuri Alexeev, Kenneth R. Brown, Frederic T. Chong, HPCA, 2020
### 🔹 Quantum Circuit Analysis 🔹 ### 
+ [QuCT: A Framework for Analyzing Quantum Circuit by Extracting Contextual and Topological Features](https://dl.acm.org/doi/10.1145/3613424.3614274) - Siwei Tan et al., MICRO, 2023
+ [Quantum Vulnerability Analysis to Guide Robust Quantum Computing System Design](https://arxiv.org/pdf/2207.14446) - Fang Qi et al., 2023



</br></br>
## 5. Error Mitigation and Correction (Quantum Error Correction, Noise-Aware Compilation)
**Keywords** : Surface code, Fault tolerance, Noise modeling


</br></br>
## 6. Hardware Execution (Pulse-Level Control, Hardware-aware compilation, Quantum ISA Design)
**Keywords** : Pulse scheduling, Optimal control, Fidelity optimization, Quantum ISA
### 🔹 Quantum ISA 🔹 ### 
+ [OpenQASM 3: A Broader and Deeper Quantum Assembly Language](https://dl.acm.org/doi/10.1145/3505636) - Andrew cross, et al., Transactions on Quantum Computing, 2022
+ [Open quantum assembly language](https://arxiv.org/abs/1707.03429) - Andrew W. Cross, Lev S. Bishop, John A. Smolin, Jay M. Gambetta, 2017
+ [A Practical Quantum Instruction Set Architecture](https://arxiv.org/abs/1608.03355) - Robert S. Smith, Michael J. Curtis, William J. Zeng, 2017


</br></br>
## Verification and Evaluation

- Quantum Circuit Verification: Circuit verification, Formal verification
- Quantum Compiler Benchmarking: Compiler benchmarking, Performance evaluation

</br></br>
## Simulation and Testing

- Quantum Circuit Simulation: Circuit simulation, Statevector simulation
</br></br>



## Related-repos
+ [Awesome-Quantum-Computing](https://github.com/desireevl/awesome-quantum-computing)
+ [Awesome-Quantum-Computation](https://github.com/hsavit1/Awesome-Quantum-Computation)
+ [Awesome-Quantum-Software](https://github.com/qosf/awesome-quantum-software?tab=readme-ov-file#quantum-compilers)
+ [Awesome-Quantum-Machine-Leaning](https://krishnakumarsekar.github.io/awesome-quantum-machine-learning/)
+ [Awesome-Post-Quantum](https://github.com/veorq/awesome-post-quantum)


## Books
+ [Quantum Computer Systems Research for Noisy Intermediate-Scale Quantum Computers (Synthesis Lectures on Computer Architecture)-Morgan & Claypool Publishers (2020)](https://www.amazon.com/Quantum-Computer-Systems-Intermediate-Scale-Architecture/dp/168173866X/ref=sr_1_1?crid=2K59KWTC2A6IG&dib=eyJ2IjoiMSJ9.FgRSqqg5BPKkIMPcNZN4SDxi0rLadqKNi_gKEwfnfdbx3NVbf-QqRugr0cm0gkqz.IP3MXubP83FTCTx1iDY4mGPq-3PRGX21K_rEV4QrWHU&dib_tag=se&keywords=Quantum+Computer+Systems+Research+for+Noisy+Intermediate-Scale+Quantum+Computers&qid=1711388706&s=books&sprefix=quantum+computer+systems+research+for+noisy+intermediate-scale+quantum+computers%2Cstripbooks-intl-ship%2C337&sr=1-1)


## Useful Learning Resources and Articles
+ [QuTech Academic](https://www.qutube.nl/)
+ [The Quantum Insider](https://thequantuminsider.com/) 
+ [Google Quantum AI](https://quantumai.google/)

## Conference
 + HPCA, ASPLOS, ISCA, MICRO, ICCAD, DAC, CC, PLDI </br>
 + QCE(Quantum Computing and Engineering) </br>
 + CF(Computing Frontiers)

## Journal
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



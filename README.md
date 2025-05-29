# Hands-On QubiC - IPDPS 2025

## Introduction
QubiC is an open-source RFSoC-based control system developed at Lawrence Berkeley 
National Laboratory for superconducting quantum processing unit (QPU). This hands-on 
tutorial provides a comprehensive overview of QubiC's architecture and capabilities, 
focusing on the unique challenges of controlling superconducting qubits. We'll also 
explore advanced features like real-time decision-making, flexible hardware integration, 
and AI/ML-powered calibration and measurement.

Participants will gain practical experience through hands-on exercises on 
1. Basic pulse-level example 
2. Gate-level QPU control and readout using QuTiP-integrated emulator 
3. Explore classical control constructs (such as loops and branch) in quantum algorithm
4. Review advanced classical design features such as AI/ML, randomization, and parameterization on FPGA for novel quantum control co-design

## When
The tutorial repeats on two days: 
- June 3rd, 8:30 AM - 12:30 PM 
- June 4th, 12:45 PM - 4:45 PM

## System Requirements and Installation
This is a hands-on tutorial, and we encourage attendees to perform some 
minimal python package installation to run the simulator.
- The laptop should have some Python environment 3.10 or above
- Install the qubic simulator package using the below command:

           pip install lbl-qubic

- Clone the tutorial git repo using below command
git clone [https://gitlab.com/LBL-QubiC/qubictutorial.git](https://gitlab.com/LBL-QubiC/qubictutorial.git)


## Topics

| Topics | Approx. time  (in min.) | Materials |
| ------ | ------ | ------ |
| Introduction to Quantum Computing | 30 | |
| Installation instruction | 15 | |
|** Part 1: Introduction to QubiC** |
| Basic pulse demo | 15 | |
|QuTip simulation|30||
|**Part 2: Exploring classical construct**s|||
|Branching - mid circuit measurement (MCM)|20||
|Loops - parameter sweeps|20||
|**Part 3: Advanced features **|
|Qiskit Integration|30||
|_**Demo only**_|
|Randomized compiling|15|[https://arxiv.org/html/2406.13967v1](https://arxiv.org/html/2406.13967v1)|
|Parameterized circuit execution|15|[https://arxiv.org/html/2409.03725v1](https://arxiv.org/html/2409.03725v1)|
|ML state descrimination|15|[https://arxiv.org/html/2406.18807v2](https://arxiv.org/html/2406.18807v2)|
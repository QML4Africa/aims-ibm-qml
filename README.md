# aims-ibm-qml
Quantum Machine Learning (QML) Hands-on Workshop curated for AIMS!  This hands‑on series will introduce you to quantum computing, and QML concepts and practical coding exercises using Qiskit and related quantum tools. Please start with the Lab 0 Activation Notebook.


Hosts: Lebohang Mashatola, Aviwe Kohlakola, Ndivhuwo Nyase, Bonga Njamela, Waheeda Saib, Stephanie Muller, Fabio, Christina, Voica
Date: 26 October 2025
Time: 15:00 - 18:00
Place: 7 Melrose Rd, Muizenberg, Cape Town, South Africa

The main goal of this session is to demonstrate how IBM Research scientists leverage Qiskit Patterns to execute QML workflow. We demonstrate an implementation of Variational Quantum Classifiers (VQCs) in labeling unseen images from the well-known IRIS dataset. 


## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Setup & Installation](#setup--installation)
4. [Workshop Structure](#workshop-structure)
5. [Exercise 1: Activation Workshop](#exercise-1-getting-started)
   - [1.1 Bell State](#12-bell-state)
   - [1.2 Superposition](#11-superposition)
   - [1.3 GHZ State](#13-ghz-state)
6. [Exercise 2: Quantum Machine Learning](#qml)



## Introduction

Quantum Computing harnesses quantum mechanics including superposition, entanglement, and interference to perform computations beyond classical limits. Quantum Machine Learning (QML) blends these quantum computing principles with machine learning to tackle problems that are intractable on classical systems. Over this workshop, you'll learn how to build, simulate, and run simple quantum circuits using Qiskit, culminating in basic QML models.


## Prerequisites

- **Python <=3.11+** installed
- **Conda** or **virtualenv** recommended
- **Git** for cloning repos
- Basic familiarity with Python programming

## Setup & Installation

1. Clone the workshop repository:
   ```bash
   git clone https://github.com/QML4Africa/csir-ibm-qml.git
   cd csir-ibm-qml
   ```
2. Create and activate a virtual environment:
   ```bash
   conda create -n qml4africa python=3.12
   conda activate qml4africa
   ```


## Workshop Structure

In this workshop You will:

- Understand basic quantum concepts like superposition
- Explore fundamental quantum gates, circuits and explore the bloch sphere.
- Simulate on Aer simulators and run on IBM Quantum hardware
- Progress to simple QML models using the IRIS dataset by the end of the series

## Lab 0: Activation Workshop

In this first exercise, you will build foundational quantum circuits:

### 1.1 Bell State

- **Objective:** Entangle two qubits to form a Bell (EPR) pair.
- **Steps:**
  1. Create a 2-qubit circuit with 2 classical bits.
  2. Apply `H` to qubit 0.
  3. Apply `CX` (CNOT) from qubit 0 → qubit 1.
  4. Measure both qubits and visualize the histogram (expect `00` and `11` only).
  
### 1.2 Superposition

- **Objective:** Prepare a single qubit in an equal superposition of |0⟩ and |1⟩.
- **Steps:**
  1. Create a 1-qubit circuit with 1 classical bit.
  2. Apply the Hadamard gate (`H`) to qubit 0.
  3. Measure the qubit into the classical bit.
  4. Simulate with 1024 shots and plot the histogram of outcomes (expect \~50% 0 and 50% 1).

### 1.3 GHZ State

- **Objective:** Extend entanglement to three qubits, creating a GHZ state.
- **Steps:**
  1. Create a 3-qubit circuit with 3 classical bits.
  2. Apply `H` to qubit 0.
  3. Apply `CX` from qubit 0 → qubit 1, then `CX` from qubit 1 → qubit 2.
  4. Measure all qubits and plot (expect `000` and `111`).


## Lab 2: Introduction to the QML using IRIS dataset

  In this exercise, we will demonstrate quantum computing and machine learning (ML) concepts explored during conference and help participants to consolodate their knowledge of QML. Using a quantum machine learning model we will predict the iris dataset.

3.1 Loading Classical Data onto a Quantum Circuit
3.2 Apply the Quantum Neural Network or Ansatz

## What is Qiskit Machine Learning?

Qiskit Machine Learning introduces fundamental computational building blocks, such as Quantum 
Kernels and Quantum Neural Networks, used in various applications including classification 
and regression.

The Qiskit Machine Learning framework aims to be:

* **User-friendly**, allowing users to quickly and easily prototype quantum machine learning models without 
    the need of extensive quantum computing knowledge.
* **Flexible**, providing tools and functionalities to conduct proof-of-concepts and innovative research 
    in quantum machine learning for both beginners and experts.
* **Extensible**, facilitating the integration of new cutting-edge features leveraging Qiskit's 
    architectures, patterns and related services.


- **Resources:**
  - Qiskit Documentation: [https://qiskit.org/documentation](https://qiskit.org/documentation)
  - IBM Quantum Experience: [https://quantum-computing.ibm.com](https://quantum-computing.ibm.com)

Happy quantum computing! 🚀


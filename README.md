# Quantum Computational Chemistry: A Promising Application for Quantum Computers

Master's Thesis in Physics of Complex Systems, University of Turin (2021/2022)

## Author
**Davide Bincoletto**

## Supervisors
- **Advisor**: Prof. Alberto Carlini
- **Co-advisor**: Dr. Alberto Acuto
- **Review Committee**: Prof. Leonardo Castellani

## Abstract

This thesis explores the intersection of quantum computing and computational chemistry, examining how quantum computers can solve complex molecular simulation problems that are intractable for classical computers. The work covers theoretical foundations, classical methods (DFT), and quantum algorithms for simulating chemical systems on both fault-tolerant and NISQ devices.

## Structure and Topics

### Introduction
Overview of computational chemistry challenges and the promise of quantum computing for solving them.

### Chapter 1: Quantum Computational Chemistry
- **Motivation**: Difficulty of simulating atomic systems by solving the Schrödinger equation (TDSE and TISE)
- **Multi-electron Hamiltonians**: Mathematical formulation and combinatorial complexity growth
- **Born-Oppenheimer approximation**: Separation of electronic and nuclear wave functions
- **Electronic structure problem**: Computing potential energy surfaces (PES) iteratively
- **Applications**:
  - Geometry optimization and stable structure identification
  - Chemical reaction mechanisms and transition states
  - Enzyme active sites with multiple coupled transition metals
  - Transition metal nanocatalysts and surface catalysts
  - Light harvesting and vision processes in conjugated organic molecules
  - Quantum molecular spectroscopy
  - High-temperature superconductivity characterization
  - Materials quantum dynamics and electron transport

### Chapter 2: Density Functional Theory (DFT)
- **Electron density approach**: Advantages over wave function methods (reduction from 3N to N variables)
- **Thomas-Fermi model**: Classical approach with kinetic and potential energy functionals
- **Exchange corrections**: Slater exchange, Thomas-Fermi-Dirac model
- **Hohenberg-Kohn theorems**: 
  - Existence theorem: ground state density determines external potential
  - Variational theorem: variational principle for electron density
- **Kohn-Sham self-consistent field method**: Non-interacting electron system reproducing real system density
- **Comparison with Hartree-Fock molecular orbital theory**

### Chapter 3: Quantum Computing Fundamentals
- **Historical development**: From Bell's inequality experiments to modern quantum computers
- **Church-Turing thesis**: Classical vs quantum computation models and computational complexity
- **Key algorithms**: Shor's factoring algorithm, Grover's search algorithm
- **Quantum supremacy**: Google's Sycamore processor demonstration (2019)
- **Qubits**: 
  - Mathematical representation in Hilbert space
  - Superposition and Bloch sphere representation
  - Multi-qubit systems and tensor products (2^N dimensional state space)
  - Coherence, decoherence, and mixed states (density matrix formalism)
  - Physical vs logical qubits distinction
- **Quantum gates and circuits**: Digital quantum computing paradigm

### Chapter 4: Quantum Computing for Computational Chemistry - FTQC Devices
- **Fault-tolerant quantum computing**:
  - Error correction codes (bit-flip, sign-flip, Shor code)
  - Encoded gates and fault-tolerance conditions
  - Threshold theorem: error probability must be below ~10⁻⁵-10⁻⁶
  - Concatenated encoding schemes for arbitrary accuracy
- **DiVincenzo's criteria**: Seven requirements for building quantum computers
- **Quantum Phase Estimation (QPE) algorithm**:
  - Eigenvalue estimation for unitary operators
  - Two-register architecture (ancilla register + system register)
  - Application to finding energy eigenvalues of molecular Hamiltonians
  - Fermionic-to-qubit mappings and Pauli string representations
  - Hartree-Fock wave function as initial state approximation

### Chapter 5: Quantum Computing for Computational Chemistry - NISQ Devices
- **NISQ era characteristics**: 50-100 noisy qubits without error correction
- **Circuit depth limitations**: ~1000 gates maximum due to noise accumulation
- **Variational Quantum Eigensolver (VQE)**:
  - Hybrid quantum-classical algorithm structure
  - Rayleigh-Ritz variational principle
  - Algorithm components:
    1. Hamiltonian construction and representation
    2. Fermionic-to-spin encoding (Jordan-Wigner, Bravyi-Kitaev, etc.)
    3. Ansatz design and state preparation (expressibility and trainability)
    4. Measurement strategies and Pauli grouping
    5. Classical parameter optimization
    6. Error mitigation techniques
  - Encoding features: qubit count, Pauli weight, number of Pauli strings
  - Barren plateaus problem in variational optimization

### Chapter 6: Computational Advantage
- **Quantum benchmarking metrics**:
  - **Scale**: Number of qubits determining solvable problem size
  - **Quality**: Quantum Volume (QV) measuring circuit fidelity
  - **Speed**: Circuit Layer Operations Per Second (CLOPS)
- **Benchmarking pyramid**: From hardware metrics to application-level benchmarks
- **IBM quantum processors**: Technical parameters including:
  - Connectivity maps and qubit topology
  - Decoherence times (T₁, T₂)
  - Gate fidelities and readout errors
  - SPAM (state-preparation-and-measurement) errors
- **Technology roadmaps**: IBM, Google, and industry projections for scaling
- **Current state**: Comparison of available processors (IBM Washington 127-qubit, Quantinuum H1-2 with QV=4096)

### Conclusion
Summary of findings and future perspectives on quantum computational chemistry.

### Acknowledgments

## Compilation

This document is written in LaTeX. To compile the thesis:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Or use `latexmk` for automatic compilation:

```bash
latexmk -pdf main.tex
```

## Files

- `main.tex` - Main LaTeX document
- `titlepage.tex` - Title page
- `dedication.tex` - Dedication page
- `usepackages.tex` - Package imports
- `bibliography.bib` - Bibliography references
- `chapters/` - Chapter source files
- `figures/` - Images and diagrams

## Output

The compiled PDF (`main.pdf`) contains the complete thesis with all chapters, bibliography, and figures.

## License

Academic thesis - University of Turin, 2022

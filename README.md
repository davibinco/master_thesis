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
Introduces the electronic structure problem, the Born-Oppenheimer approximation, and key application areas where quantum computing can impact chemistry.

### Chapter 2: Density Functional Theory (DFT)
Covers the foundations of DFT, including the Thomas-Fermi model, Hohenberg-Kohn theorems, and the Kohn-Sham method for practical calculations.

### Chapter 3: Quantum Computing Fundamentals
Explains qubits, quantum gates, entanglement, and landmark algorithms like Deutsch-Jozsa, Grover's, and Shor's algorithm.

### Chapter 4: Fault-Tolerant Quantum Computing
Discusses quantum error correction, the threshold theorem, and the Quantum Phase Estimation (QPE) algorithm for chemical applications.

### Chapter 5: NISQ Devices and VQE
Details the Variational Quantum Eigensolver (VQE) algorithm, its components, qubit encoding strategies, and challenges like barren plateaus in noisy intermediate-scale quantum devices.

### Chapter 6: Computational Advantage
Presents benchmarking metrics like Quantum Volume and CLOPS, along with specifications of current IBM quantum processors and future technology roadmaps.

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

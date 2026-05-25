# Computación cuántica y las desigualdades de Bell

**Master's Thesis Protocol in Physics**  
**Author:** Lic. Julio A. Medina  
**Institution:** Escuela de Ciencias Físicas y Matemáticas, Universidad de San Carlos de Guatemala  
**Topic:** Quantum computing, Bell inequalities, CHSH inequality, quantum entanglement, and Qiskit-based experimentation.

---

## Overview

This repository contains the thesis protocol **"Computación cuántica y las desigualdades de Bell"**, a master's-level research proposal focused on the theoretical foundations of quantum computing and their connection with Bell's theorem, quantum entanglement, and the CHSH inequality.

The project combines a rigorous study of quantum mechanics with practical implementations using **Python** and **Qiskit**. A central goal is to move from mathematical derivations to executable quantum circuits, including simulations and experiments on real IBM quantum hardware when available.

The protocol is written in Spanish and developed in LaTeX.

---

## Research Motivation

Quantum computing represents a radically different computational paradigm from classical computing. Instead of relying only on classical bits, quantum computers use **qubits**, whose behavior is governed by superposition, measurement, and entanglement.

The protocol is motivated by the idea, originally emphasized by Richard Feynman, that classical computers face severe limitations when simulating intrinsically quantum systems. Quantum devices may therefore become essential tools for studying many-body systems, quantum algorithms, optimization problems, and future applications in artificial intelligence.

A key part of this research is the study of **Bell inequalities**, especially the **CHSH inequality**, as a way to understand and test one of the most important consequences of quantum mechanics: the incompatibility between local hidden-variable theories and quantum predictions.

---

## Main Objective

To understand the current state of quantum computing and evaluate possible future research directions, including doctoral-level work in quantum computing or related areas such as **Quantum Machine Learning**.

---

## Specific Objectives

The thesis protocol proposes to:

1. Study the basic principles of quantum computing through advanced quantum mechanics.
2. Derive Bell inequalities and understand their physical significance.
3. Build familiarity with the theoretical tools used in quantum computation.
4. Study basic quantum algorithms such as Shor's algorithm and Deutsch-Jozsa.
5. Translate mathematical formulations of quantum algorithms into Python implementations using Qiskit.
6. Analyze the relationship between Bell inequalities and the CHSH inequality.
7. Use a real quantum computer to test the CHSH inequality and experimentally illustrate Bell's theorem.

---

## Theoretical Topics Covered

The protocol develops the theoretical background needed to connect quantum mechanics with quantum computing. The main topics include:

### Quantum Mechanics Foundations

- Dirac notation
- Bra-ket notation and inner products
- Hilbert spaces
- Qubit representation
- Pauli matrices
- Quantum measurement
- Born rule
- Spin measurements

### Entanglement and Bell Inequalities

- Spin-singlet states
- Einstein-Podolsky-Rosen correlations
- Locality and hidden-variable theories
- Bell's theorem
- Bell inequality derivations
- CHSH inequality
- Quantum violations of classical bounds

### Quantum Computing

- Qubits and quantum gates
- Hadamard gate
- Pauli gates
- Quantum Fourier Transform
- Relationship between QFT and the Hadamard transform
- Basic quantum algorithm implementation ideas

### Applied Direction

- Qiskit-based simulations
- Execution on IBM quantum hardware
- Noise and hardware error analysis
- Introductory exploration of Quantum Machine Learning

---

## Methodology

The project follows a hybrid methodology:

1. **Theoretical development**  
   The relevant quantum mechanical results are derived from first principles, with special attention to Bell inequalities, spin correlations, and quantum information concepts.

2. **Computational implementation**  
   The mathematical formulations are translated into Python code using Qiskit. This includes basic quantum circuits, simulations, and potentially executions on real IBM quantum computers.

3. **Reproducibility through GitHub**  
   Code, figures, LaTeX source files, and results should be versioned in this repository so the thesis development remains transparent and reproducible.

4. **Experimental validation**  
   The CHSH inequality is proposed as a concrete experiment for comparing classical expectations with quantum-mechanical predictions.

---

## Suggested Repository Structure

A clean structure for this project could look like:

```text
.
├── README.md
├── Protocolo.tex
├── figures/
│   └── spin_correlation_spin_singlet.png
├── notebooks/
│   ├── 01_dirac_notation_examples.ipynb
│   ├── 02_bell_chsh_simulation.ipynb
│   └── 03_qft_examples.ipynb
├── src/
│   ├── bell_chsh.py
│   ├── qft.py
│   └── qiskit_utils.py
├── results/
│   ├── simulations/
│   └── hardware_runs/
├── references/
└── build/
```

This structure separates the thesis document, code, notebooks, figures, and generated outputs.

---

## How to Compile the Thesis Protocol

The thesis protocol is written in LaTeX. To compile it locally, make sure a LaTeX distribution is installed, such as **TeX Live** on Linux.

### Basic compilation

```bash
pdflatex Protocolo.tex
```

Run the command more than once if references, labels, or the table of contents need to be updated:

```bash
pdflatex Protocolo.tex
pdflatex Protocolo.tex
```

### Notes

The document currently depends on standard LaTeX packages such as:

- `babel`
- `amsmath`
- `amsfonts`
- `amssymb`
- `graphicx`
- `hyperref`
- `booktabs`
- `algorithm`
- `algpseudocode`

The file also references the figure:

```text
spin_correlation_spin_singlet.png
```

Make sure this image is available in the expected path before compiling.

---

## Suggested Qiskit Workflow

A practical development workflow could be:

```bash
python -m venv .venv
source .venv/bin/activate
pip install qiskit qiskit-aer matplotlib numpy scipy jupyter
```

Then run notebooks or scripts from the repository:

```bash
jupyter notebook
```

For IBM Quantum hardware experiments, credentials and backend access should be configured following the current IBM Quantum/Qiskit Runtime workflow.

---

## Possible Computational Experiments

The thesis can be strengthened by adding reproducible experiments such as:

1. **CHSH simulation with ideal quantum circuits**  
   Build a Bell pair, measure correlations in different bases, and compute the CHSH parameter.

2. **CHSH experiment with noisy simulation**  
   Compare the ideal result with a noisy backend simulation.

3. **CHSH experiment on IBM hardware**  
   Run the same circuit on a real quantum device and analyze how noise affects the violation.

4. **Quantum Fourier Transform notebook**  
   Implement the QFT for small numbers of qubits and compare the circuit output with the theoretical derivation.

5. **Introductory Quantum Machine Learning exploration**  
   Add a small, clearly bounded example connecting quantum circuits with classical machine learning workflows.

---

## Key References

The protocol cites foundational works and standard texts, including:

- J. S. Bell, *On the Einstein Podolsky Rosen Paradox*.
- J. F. Clauser, M. A. Horne, A. Shimony, and R. A. Holt, *Proposed Experiment to Test Local Hidden-Variable Theories*.
- A. Einstein, B. Podolsky, and N. Rosen, *Can Quantum-Mechanical Description of Physical Reality be Considered Complete?*
- R. P. Feynman, *Simulating Physics with Computers*.
- P. W. Shor, *Polynomial-Time Algorithms for Prime Factorization and Discrete Logarithms on a Quantum Computer*.
- M. A. Nielsen and I. L. Chuang, *Quantum Computation and Quantum Information*.
- J. J. Sakurai, *Modern Quantum Mechanics*.
- N. David Mermin, *Quantum Computer Science: An Introduction*.
- Qiskit documentation and textbook resources.

---

## Suggestions for Improving the Thesis Protocol

The current protocol already has a strong theoretical direction. These are recommended improvements for the next iteration:

### 1. Add a concise abstract

The LaTeX file has an abstract section commented out. Adding a short abstract would make the protocol easier to evaluate academically.

### 2. Clarify the research question

The document has clear objectives, but it would benefit from one explicit guiding research question, for example:

> How can the CHSH inequality be theoretically derived and experimentally tested using Qiskit simulations and IBM quantum hardware?

### 3. Separate theoretical and computational deliverables

It would help to distinguish between:

- mathematical derivations,
- Qiskit simulations,
- real-hardware executions,
- analysis of noisy results,
- possible Quantum Machine Learning extensions.

### 4. Update and clean the bibliography

There is a duplicated `Qiskit` bibliography entry. Also, a few references could be modernized by adding recent Qiskit Runtime documentation and recent CHSH or quantum-hardware experiment references.

### 5. Add a timeline

A thesis protocol usually benefits from a short schedule showing when the literature review, derivations, simulations, hardware experiments, and writing will be completed.

### 6. Add reproducibility criteria

Since the methodology depends on GitHub and Qiskit, define what counts as a reproducible result:

- fixed package versions,
- saved backend metadata,
- saved circuit diagrams,
- stored measurement counts,
- scripts or notebooks that regenerate figures.

### 7. Polish minor language issues

The Spanish text is understandable and technically strong, but a final pass should fix small typos and wording issues, such as repeated words, accent marks, and phrases like `ordenar cuántico`, which should likely be `ordenador cuántico` or `computadora cuántica`.

---

## License

No license has been specified yet. If this repository will be public, consider adding a license file. For an academic thesis repository, common options are:

- MIT License for code,
- Creative Commons license for text,
- or a custom notice if the thesis text should remain under institutional restrictions.

---

## Status

This repository is currently at the **thesis protocol / research design** stage. The next natural step is to organize the computational experiments and align them with the theoretical sections of the document.

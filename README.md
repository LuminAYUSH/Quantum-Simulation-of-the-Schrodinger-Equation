# Quantum Simulation of the Schrödinger Equation

## Project Overview
This project explores the quantum simulation of the Schrödinger equation for various **one-dimensional potentials** using **Qiskit**, a quantum computing framework. Leveraging the power of quantum computing, the study simulates a range of potentials, including:
- Free particle
- Infinite square well
- Simple harmonic oscillator (SHO)
- Quantum tunneling
- Two-particle interaction system

The simulations provide insights into quantum phenomena such as **confinement**, **tunneling**, and **energy quantization**.

---

## Key Features
- **Simulated Potentials**:
  - Free particle: Probability density evolution without potential.
  - Infinite square well: Eigenstates with no tunneling effects.
  - SHO: Quantum harmonic oscillator wavefunctions and energy quantization.
  - Quantum tunneling: Tunneling through barriers for Gaussian wave packets.
  - Two-particle interaction: Interactions with a Dirac delta potential.
- **Quantum Computing Tools**:
  - Implementation using **Qiskit**.
  - Simulation conducted on **Statevector** and **QASM simulators**.
- **Quantum Circuits**:
  - Time evolution circuits utilizing the **Quantum Fourier Transform (QFT)**.

---

## Methodology

### Schrödinger Equation
The time-dependent Schrödinger equation is given by:
$$H|\psi(t)\rangle = i\hbar \frac{\partial}{\partial t}|\psi(t)\rangle$$
For a time-independent Hamiltonian:
$$H = K + V = \frac{p^2}{2m} + V$$
Simulations use the **Trotter-Suzuki decomposition** to approximate time evolution.

### Quantum Circuit Design
1. **Initialization**:
   - Gaussian wave packets used to initialize states.
   - Discretization over qubits for position-space representation.
2. **Kinetic Energy Operator**:
   - Momentum-space implementation via **QFT**.
3. **Potential Operator**:
   - Encodes potentials such as infinite wells, harmonic oscillators, and barriers.

---

## Experiments
### 1. Free Particle
- Simulated a particle with no potential $V = 0$.
- Results demonstrate the spreading of the wave packet over time.
  
### 2. Infinite Square Well
- Modeled using a high potential barrier $V \to \infty$ at the boundaries.
- Observed reflections with no tunneling effects.

### 3. Quantum Tunneling
- Gaussian wave packet tunneling through a potential barrier.
- Results showcase exponential decay inside the barrier and transmission/reflection phenomena.

### 4. Simple Harmonic Oscillator
- Simulated SHO potentials with quantized energy levels.
- Wavefunctions aligned with expected Hermite polynomial solutions.

### 5. Two-Particle Interaction
- Interaction potential modeled using a Dirac delta function.
- Observed dynamics of Gaussian wave packets as particles interacted and moved within a bounded region.

---

## Results
- Accurate visualization of quantum behaviors such as **tunneling**, **energy quantization**, and **particle interactions**.
- Validated the power of quantum circuits in simulating diverse quantum phenomena.

---

## Example Visuals
- **Quantum Tunneling**:
  ![Quantum Tunneling](https://github.com/user-attachments/assets/35982a09-c787-44d0-b2c9-857fa99ee941)

- **Simple Harmonic Oscillator**:
  ![SHO Wavefunctions](https://github.com/user-attachments/assets/09ad9f89-997e-4ac0-8f24-33367beec32f)
  
---

## Future Directions
- Extend simulations to **multi-dimensional quantum systems**.
- Incorporate noise models to study **decoherence** and error correction.
- Explore **quantum machine learning** techniques for pattern recognition in quantum systems.

---

## References
1. Eltohfa, M. *Quantum Simulation of Schrödinger’s Equation*.  
2. Abouelela, M. *Quantum Simulation using IBM Quantum Computers*.  
3. Benenti, G. and Casati, G. *Principles of Quantum Computation and Information*.  

---

This project underscores the potential of **quantum computing** for advancing our understanding of quantum systems and highlights its application in studying fundamental quantum phenomena.

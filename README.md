# Quantum Teleportation and Classical Routing

This project demonstrates the concept of classical routing and quantum teleportation over a network, showcasing the differences in data transmission methods. The system involves classical routing for standard data and quantum teleportation for transmitting quantum information (qubits) between nodes.

## Classical Routing

Classical routing refers to the process of sending regular (non-quantum) data across a network using conventional routing protocols. In our example, the routing path is:

- **Path**: New York → London → Tokyo
- **Time Taken**: 9.799003601074219e-05 seconds (approximately 0.000098 seconds)

This time measurement demonstrates the speed at which classical routing algorithms can determine a path through a network.

## Quantum Teleportation

Quantum teleportation is a process used to transfer quantum information (qubits) between locations using quantum entanglement. In this project, the qubits are in superposition (a combination of states 0 and 1) before measurement, where they collapse into specific states.

### Quantum States

- **'100'**: The first qubit is 1 (on), second and third qubits are 0 (off).
- **'110'**: The first and second qubits are 1 (on), third qubit is 0 (off).

These states represent the outcomes after teleporting a set of qubits from one node to another.

### Measurement and Outcomes

After quantum teleportation, the system measures the quantum state of the qubits. The measurements show how often certain states are observed after the teleportation process. For example:

- **'100': 104** means the state '100' was measured 104 times.
- **'110': 127** means the state '110' was measured 127 times.

These results highlight the probabilistic nature of quantum teleportation, where different states appear with varying frequencies.

### Entanglement and Teleportation Protocol

Before teleporting the quantum information, the nodes (e.g., New York and Tokyo) are entangled. This means the qubits at these nodes are connected such that measuring one qubit will instantaneously affect the other.

- The teleportation process uses both classical and quantum processes to transfer the qubit.
- **Entanglement**: Pre-existing entanglement between nodes enables the quantum state transfer.
- **Measurement and Feedback**: After measuring the qubit's state at New York, the result is communicated to Tokyo via classical routing (Python’s socket communication), and Tokyo uses this information to reconstruct the qubit, completing the teleportation.

### Resulting Quantum States

After teleportation, quantum states like '100', '110', etc., represent the final state of the qubits after the process. These states occur probabilistically, with some states more likely than others.

## Key Concepts

- **Classical Routing**: Standard data transmission across a network, with results measured in nanoseconds.
- **Quantum Teleportation**: The transfer of quantum information using entanglement, followed by classical feedback and measurement.
- **Entanglement**: A quantum phenomenon where qubits at different locations are linked, affecting each other instantaneously.

## Conclusion

This project illustrates the differences between classical routing and quantum teleportation in data transmission. Classical routing is fast and deterministic, while quantum teleportation relies on probabilistic measurements and quantum entanglement.
"""

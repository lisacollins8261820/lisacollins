# Lisacollins

Lisacollins is a Node.js module providing a collection of utility functions for quantum computing simulations.

## Installation

You can install Lisacollins via npm: `npm install lisacollins`

## Usage
```javascript
const quantumUtils = require('quantum-utils');

// Example usage of the functions
const numQubits = 2;
const gates = [
    { type: 'H', targets: [0] },
    { type: 'CX', targets: [0, 1] }
];
const state = quantumUtils.simulateQuantumCircuit(numQubits, gates);
console.log('Simulated quantum circuit result:', state);

const randomState = quantumUtils.generateRandomState(3);
console.log('Generated random quantum state:', randomState);

const entropy = quantumUtils.calculateEntanglementEntropy(randomState);
console.log('Entanglement entropy of the random state:', entropy);
```
# POLY-PROOF_MOD_3
# My Circom Circuit Template for Multiplication Checking

Hello everyone! 

I am excited to share my Circom circuit template that checks whether 'c' is the result of multiplying 'a' and 'b'. This circuit is implemented using the version 2.0.0 of the Circom language.

## Getting Started

## Circuit Description

The circuit uses three main gates: AND gate, NOT gate, and OR gate, which are defined as templates. The custom CircomCircuit template wires these gates together to create the final multiplication checking circuit.

### AND Gate (template: AND)

The AND gate takes two input signals, A and B, and produces the output signal out. The output out is computed as the logical AND of A and B, i.e., out = A * B.

### NOT Gate (template: NOT)

The NOT gate has one input signal, 'in', and produces one output signal, 'out'. The output 'out' is computed as the logical negation of the input 'in', i.e., out = 1 + in - 2*in.

### OR Gate (template: OR)

The OR gate takes two input signals, A and B, and produces the output signal out. The output 'out' is computed as the logical OR of A and B, i.e., out = A + B - A*B.

### Custom Circuit (template: CircomCircuit)

The custom CircomCircuit template takes two input signals, A and B, representing the numbers to be multiplied. It uses the previously defined AND, NOT, and OR gates to perform the multiplication checking. The intermediate signals x and y are used to store temporary results. Finally, the output signal q holds the result of whether 'c' is the product of 'a' and 'b'.

## How to Use

The circuit uses basic logic gates (AND, NOT, and OR) to determine the validity of the multiplication. Here's a brief explanation of the logic:

The input signals A and B are provided as inputs to the circuit.

An AND gate (ANDg) takes inputs A and B, producing an intermediate signal x, which represents the logical AND of A and B.

The NOT gate (NOTg) takes input B and produces an intermediate signal y, which represents the logical NOT of B.

An OR gate (ORg) takes inputs x and y, producing the output signal q, which represents the logical OR of x and y.

The final output signal q will be 1 if and only if c is the multiplication of a and b

## Author

SATYA PRAKASH

## License

This project is under MIT license

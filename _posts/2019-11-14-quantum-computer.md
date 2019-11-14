---
layout: post
comments: true
title: Introduction to quantum computing
---

Quantum Supremacy means that quantum computers could efficiently solve a computational problem 
that a classical computer can only solve inefficiently. The question is can we achieve quantum
supremacy in the near future? The answer is **NO**, but many industrial giants are betting on quantum computing.

## What is a quantum computer?

In a classical computer, information is stored in bits that are always either 0 or 1. Note that 1 byte = 8 bits.
A logic gate is an operator acting on bits.
In mathematics, bits and gates can be represented by Boolean algebra and operations.
It is easy to obtain stable bits in nature, for instance,
an electron can be spin up or spin down; a photon can be left-handed or right-handed in its polarization.

Based on quantum mechanics, we have enough knowledge, at least in physics and mathematics, for building a quantum computer,
but the difficulty is mainly in material science and engineering.
A quantum computer uses quantum bits, or qubits.
A qubit is a two-state quantum mechanical system, meaning a qubit is generally in a coherent superposition of those two pure states as a basis.
For a system of n qubits, the space of quantum states can be represented by an n-dimensional Hilbert space.
A (reversible) unitary transformation of a quantum state is then represented as a unitary matrix, so that possible operations on qubits
are embedded into a matrix algebra. A universal set of quantum logic gates is a set of generator matrices.
Qubits together with quantum gates are the building blocks of quantum circuits.
It is really hard to manipulate qubits and quantum gates, there are different experiments trying to build a scalable quantum computer.

In quantum mechanics, a measurement changes the quantum state of a qubit.
For instance, standard basis measurement is an irreversible operation in which information is gained about the state of a qubit.
In a ground and excited two-state system, a qubit that is in an excited state will decay back to the ground state
on a timescale known as the coherence time.
If one of your qubits decays before all of your computations are performed and you read out your answer,
that will create an error.
Quantum entanglement, which is a nonlocal property of two or more qubits that allows a set of qubits to express higher correlations,
 is another important feature to consider when designing quantum gates.

Many possible qubits and gates have been designed and even implemented physically, David DiVincenzo
proposed five criteria to assess various implementations.
* Measurable: the quantum output can be read out.
* Universal: a feasible universal set of quantum logic gates so arbitrary quantum algorithms can be expressed as a sequence of these gates.
* Scalable: the computer can be enlarged to more qubits and quantum gates with low enough cost that the quantum advantage is not removed.
* Initializable: the qubit string can be prepared all in the (∣0〉) state.
* Coherent: quantum logic operations are sufficiently impervious to decoherence so quantum error correction strategies work with scalable overhead.

Some notable experiments have been performed in superconducting systems, ion-traps, quantum dots and photonic systems etc.
For example, a trapped ions quantum computer uses lasers to change the energy level of laser-cooled ions trapped
in an electric field.
From my background in condensed matter physics, I will talk more about superconducting systems and topological quantum computers below.

## Superconducting quantum computing

Superconductivity is a standard chapter in a modern condensed matter physics textbook.
Superconducting quantum computing is an implementation of a quantum computer in superconducting electronic circuits.
Physicists are still looking for new superconductors, but high temperature superconductivity is rare in nature.
Superconducting quantum computers have good coherence times, but such systems have to be operated at extremely low temperatures.

In a superconductor, the basic charge carriers are pairs of electrons known as Cooper pairs.
When the temperature drops below a critical value, two electrons form a weak bound and becomes a Cooper pair
that experience no resistance when traveling through the metal.  The pairing opens a gap in the continuous spectrum of allowed energy states of the electrons,
 meaning that all excitations of the system must possess some minimum amount of energy.
This gap leads to superconductivity since not any random increase in energy is allowed.

The three superconducting qubit archetypes are the charge, flux and phase qubits, and there are many hybrids based on those three.
For any qubit implementation, the quantum states |0>, |1> are to be mapped to the different states of the physical system,
typically to the discrete energy levels or to their superpositions.
In the charge qubit, a qubit is a superconducting-circuit with a Cooper pair of electrons on the left (∣0〉) or right (∣1〉) of a Josephson barrier.
To make the spacing unequal for energy levels, a Josephson junction is placed into the circuit.
In the flux qubit, the downward magnetic flux serves as ∣0〉 and the upward flux as ∣1〉,
since the magnetic flux is quantized  in a superconducting loop.
In the phase qubit, the energy levels correspond to different quantum charge oscillation amplitudes across a Josephson junction.

An arbitrary single qubit gate is achieved by rotation in the Bloch sphere. Coupling qubits is essential for implementing 2-qubit gates.
Coupling two qubits may be achieved by connecting them to an intermediate electrical coupling circuit.
Another method of coupling two or more qubits is by coupling them to an intermediate quantum bus.

## Topological quantum computing
A topological quantum computer is a _theoretical_ quantum computer that employs two-dimensional quasiparticles called anyons,
whose world lines pass around one another to form braids in a three-dimensional spacetime.
In topological quantum computing, qubits are initialized as non-abelian anyons,
operations are performed upon qubits through braiding the worldlines of the anyons, that is,
these braids form the quantum logic gates. Finally, a measurement is taken by fusing the particles.

The involved interesting mathematics are braid groups, fusion rules, and braided fusion categories.
Anyon fusion is the process by which multiple anyons fuse into another type of anyons. 
Non-abelian anyons means the fusion rules are noncommutative, of course, abelian anyons are easier in theory. 

While topological quantum computing originates in a purely mathematical realm, experiments
in fractional quantum Hall systems indicate these elements may be created in the real world.
Topological insulators are also promising in building topological quantum computers.


## Quantum algorithms

The most well known algorithms are Shor's algorithm for factoring,
and Grover's algorithm for searching an unstructured database or an unordered list.
Shor's algorithms runs almost exponentially faster than the best known classical algorithm for factoring integers, 
in fact it is a polynomial-time quantum algorithm. 
Grover's algorithm runs quadratically faster than the best possible classical algorithm for the same task, it is 
 based on the technique of amplitude amplification.


Witten showed the Chern-Simons topological quantum field theory (TQFT) can be solved in terms of Jones polynomials.
If a quantum computer can simulate a TQFT and approximate the Jones polynomial, 
then problems in quantum topological invariants would be solved easily.


## References

Barry C Sanders, How to build a quantum computer, IOP Publishing Ltd 2017

Nayak, Simon, Stern, Freedman, and Das Sarma, Non-Abelian Anyons and Topological Quantum Computation, Reviews of Modern Physics

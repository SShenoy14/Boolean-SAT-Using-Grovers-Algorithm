# Boolean-SAT-Using-Grovers-Algorithm

# Grover's Algorithm
Grover's algorithm, also known as the quantum search algorithm, refers to a quantum algorithm for unstructured search that finds with high probability the unique input to a black box function that produces a particular output value, using just O(sqrt(N)) evaluations of the function, where N is the size of the function's domain.

# Problem Statement
Frank wants to throw a dinner party to celebrate Alice and Bob’s engagement. He is also considering inviting their mutual friends Charles, Dave and Eve. However, he is aware that Charles will come to the party only if Dave comes without Eve. Frank wants to know what possible combinations of invitations he can write for his friends Alice, Bob, Charles, Dave and Eve.

Help Frank calculate all the possible combinations using Grover’s algorithm.

# Roadmap

1) We assign a qubit to each person. We also formulate a boolean expression that satisfies the problem constraints.
2) Assuming Alice,Bob,Charles,Dave and Eve as A,B,C,D and E respectively, any combination of ABCDE that satisfies the aforementioned expression is a solution to our problem.
3) We construct a phase oracle corresponding to the above mentioned boolean expression.
4) We construct the standard reflector used in Grover's Algorithms.
5) We create the final circuit initialising the state to a uniform superposition and then sequentially apply the oracle and reflectors.
6) We calculate the number of iterations using the number of solution states and number of total states.
7) The QASM simulator is used to run the algorithm the respective number of times and we obtain the correct answer(s) with an acceptable error rate.



# Tideman-Election-Simulation

This program simulates the Tideman election algorithm, a ranked preferential voting system that determines the winner of an election based on the preferences of voters.

## Quick Start

1. Clone Repository:

`https://github.com/Kate-h36/Tideman-Election-Simulation.git`

2. Change directory where cloned program is located:

`cd___`

3. Compile the program: 

`clang -o name of the program name of the program.c -lcs50`
`make name of the_program`

4. Run the program:

`./tideman <names of candidates>`

5. Follow the instructions on the screen to enter the candidates and the voters' preferences.
6. The program will output the winner of the election.

## Usage 
1. Enter the names of the candidates.
2. Enter the number of voters.
3. For each voter, enter the rankings of the candidates.
4. The program will output the winner of the election.

```
./tideman Alice Bob Charlie
Number of voters: 5
Rank 1: Alice
Rank 2: Charlie
Rank 3: Bob

Rank 1: Alice
Rank 2: Charlie
Rank 3: Bob

Rank 1: Bob
Rank 2: Charlie
Rank 3: Alice

Rank 1: Bob
Rank 2: Charlie
Rank 3: Alice

Rank 1: Charlie
Rank 2: Alice
Rank 3: Bob

Charlie
```

## Algoritm Explanetion

The Tideman election method is a ranked voting system. Each voter ranks all candidates in order of preference. The candidate with the most top-ranked votes wins. If there is a tie, the candidate with the fewest last-ranked votes wins.

The algorithm works as follows:

Each voter ranks all the candidates.
For each pair of candidates (A, B), we count how many voters prefer A to B.
We create a graph, where each node represents a candidate, and each edge (A, B) represents the fact that more voters prefer A to B than B to A.
We sort the nodes of the graph in decreasing order of their "strength", defined as the sum of incoming edge weights minus the sum of outgoing edge weights. We break ties by sorting the candidates in lexicographic order.
We add nodes to the output list in decreasing order of strength, as long as they don't create cycles in the graph.
The winner is the candidate that appears first in the output list.

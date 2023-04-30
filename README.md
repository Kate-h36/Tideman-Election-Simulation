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

1. Enter the number of candidates.
2. Enter the names of the candidates.
3. Enter the number of voters.
4. For each voter, enter the rankings of the candidates.
5. The program will output the winner of the election.

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

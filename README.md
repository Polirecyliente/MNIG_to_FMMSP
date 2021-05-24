# Multi-Neighborhood Iterated Greedy (MNIG) algorithm, to solve the Fuzzy Multiproduct Multistage Scheduling Problem (FMMSP)

This is the MNIG algorithm written in Python to solve the FMMSP. The
MNIG algorithm is implemented here as defined by the article:
https://www.sciencedirect.com/science/article/abs/pii/S0950705120300344

The FMMSP model is defined in
https://www.sciencedirect.com/science/article/abs/pii/S0925231220302563

This implementation is at least as good as the DBSA-LS algorithm to
solve the FMMSP (as is confirmed using the only available public
instance of the FMMSP, which is the one that comes by default inside
this program).

# Usage

`python3 MNIG_to_FMMSP 5 1.1 4`

This example command makes the algorithm run 250 iterations (which comes
from $10*5^2$).

The meanings of the arguments are taken from the MNIG algorithm, they
are $N$, $T_0$, and $d$, respectively.

# Installation

Download the release and extract it. The command shown in Usage is
executed in the same directory as the one that contains the extracted program.

## Dependencies

You must have the following, already installed.

- The `python3` interpreter.
- The Numpy module

# Details about the code

The comments and the doc-strings are written in Spanish, because this
project was originally created in Spanish.

An optional `--debug` flag can be passed to the program, to print each
iteration with its sequence, the makespan of the sequence, and a few
other info. At the end of the iterations, a table is printed with the
starting times and the finish times of each job in the sequence, among
other info.

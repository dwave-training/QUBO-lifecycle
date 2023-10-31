[![Open in GitHub Codespaces](
  https://img.shields.io/badge/Open%20in%20GitHub%20Codespaces-333?logo=github)](
  https://codespaces.new/dwave-training/QUBO-lifecycle?quickstart=1)
  
# QUBO-lifecycle
Demonstrates what happens when you send a QUBO to the D-Wave QPU

## Overview

This program takes a 3-variable QUBO function and demonstrates what goes on 
"behind the scenes" as it runs on the QPU.  We see:

1. The original QUBO.
2. The equivalent Ising form.
3. The Ising form embedded onto the QPU architecture using four qubits.
4. A scaled version of the embedded Ising form that is the final QMI.

At this point, the problem is run on the D-Wave QPU.  When a solution is 
returned, we see:

5. The QMI solution (embedded Ising solution).
6. The unembedded Ising solution, with any chain breaks resolved.
7. The equivalent unembedded QUBO solution.

Note that we use the default chain strength value in this program (value of 1).  

## Exercise

First, run the program as is.  Hit return (enter) to continue to the next 
output as the program runs.

Second, consider the following 3-boxes problem.

Problem:

Pick the pair of boxes with the smallest sum.

![3-boxes problem](readme_imgs/basic_problem.png "3-boxes problem")

As a QUBO, this is written:

![3-boxes QUBO](readme_imgs/basic_qubo.png "3-boxes QUBO")

Write down your new QUBO, with the Lagrange parameter set to 24.

Third, do the algebra, and write down your new QUBO.

Fourth, in the program for this unit, replace the entries of your Q matrix, with 
the values from your new QUBO.

Fifth, run the program.

Sixth, check through the results, and make sure that you understand them,
compared to what you found in the first step.

## License

Released under the Apache License 2.0. See [LICENSE](LICENSE) file.

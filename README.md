#[woodcutter](https://github.com/781flyingdutchman/woodcutter)

##Purpose

Simple Python script to find the best way to cut pieces of fixed-length lumber into the cut lengths desired, while
minimizing waste.  Inspired by [WoodCutterBuddy](https://github.com/JOSMANC/WoodCutterBuddy), which attempts to solve
this through a more advanced algorithm (delayed column generation and a revised simplex method with a modified knapsack
solver), but which can't solve more complex cut patterns due to the NP-hard nature of the problem.

The approach in this script uses a very simple algorithm: trying to fit the largest cut in remaining lumber, and if
that's not possible, add a new piece of lumber.  While this may not yield the absolte optimal solution, it gets very
close for practical pruposes, and is very fast.

##Use

An example use is embedded in the script's __main__ section, illustrating the use with different lumber names/types
and with and without a label for each cut.

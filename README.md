This code simulates a smart self-healing power distribution system using the IEEE 33-bus radial network.
First, it downloads real-world household load data from Kaggle and selects a user-specified day for the simulation.
Then, it builds the 33-bus network using pandapower, adds residential loads, and integrates synthetic solar and wind energy generators.
A time-series simulation runs for 24 hours, updating loads and renewable generation every hour.
Artificial faults are injected at specific hours, and the system automatically detects low voltages and performs self-healing by closing a tie-switch to restore power.
Finally, it plots voltage profiles, load behavior, renewable generation output, total system losses, and fault occurrences to visualize the network’s dynamic response and healing performance.

# SNN-radiation-simulation
Simulates radiation effects on spiking neural networks. Chipset independent, assumes SEE propagation mechanisms.

## SEE propagation assumptions
Currently radiation effects, are modelled as permanent neuron death. However, the code is built modular and supports alternative radiation effect mechanisms. The following radiation effect propagation mechanisms are supported yet not yet implemented:
 - Synaptic death
 - Transient SEE effects
 - Neuronal property changes.
 - Synaptic property changes.
 
The probability of simulated propagated radiation effects is configurable, as well as the magnitude of the effects (such as neuronal property changes). This package does not currently support chip-dependent radiation effect propagation, such as memory address errors. It is tailored to radiation effects on the neuronal modules, and not on the boiler plate components such as CPU's that often still exist on neuromorphic chips. A motiviation for this design choices is limiting the scope of the research. A practical use case may be to lower the shielding and/or hardware module redundancies specificaly on these neurenal modules.


## Note
This code is currently still integrated in [this networkx LIF-neuron simulator](https://github.com/a-t-0/networkx-to-lava-nc), which is being refactored. After refactoring, the radiation simulation mechanisms will be moved into this separate repository.

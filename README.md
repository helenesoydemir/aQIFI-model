# aQIFI-model

🔬 Modeling Pathological Neural Dynamics via Mean-Field Reduction

During my internship, I worked on an extended AdEx neuron model that includes a slow variable to simulate impaired ion regulation, particularly under elevated extracellular potassium conditions [1]. This model captures pathological dynamics such as those observed in epilepsy.

🧠 The goal was to reformulate the model within the Adiabatic Quadratic Integrate-and-Fire (AQIF) framework, making it compatible with the Montbrió mean-field reduction method, and enabling its extension to the population level.

📉 This approach supports the derivation of a reduced neural mass model that preserves the essential dynamics of the original spiking network, paving the way for integration into large-scale brain simulations.

🔗 References:
[1] Depannemaecker et al., bioRxiv, 2024 – https://doi.org/10.1101/2024.08.01.606188
[2] Carlu et al., J. Neurophysiol., 2020 – https://doi.org/10.1152/jn.00399.2019

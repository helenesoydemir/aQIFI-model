# 🧠 aQIFI-model  
![Python](https://img.shields.io/badge/Python-3.10-blue)  
![License](https://img.shields.io/badge/license-MIT-green)  
![Status](https://img.shields.io/badge/status-Active-brightgreen)

## 🔬 Modeling Pathological Neural Dynamics via Mean-Field Reduction  

During my internship, I worked on an extended **AdEx neuron model** that includes a slow variable to simulate **impaired ion regulation**, particularly under **elevated extracellular potassium conditions** [1].  This model captures pathological dynamics such as those observed in **epilepsy**.

🧠 The long-term goal was to reformulate the model within the **Adaptative Quadratic Integrate-and-Fire (aQIF)** framework, making it compatible with the **Montbrió mean-field reduction** method, and enabling its extension to the population level.  In fact, this approach supports the derivation of a **reduced neural mass model** that preserves the essential dynamics of the original spiking network, paving the way for integration into **large-scale brain simulations**.

First, we will characterize this new model, identify its repertoire of interesting dynamical regimes, and finally analyze it using geometric singularity theory, fast–slow system decomposition, and bifurcation analysis.
---

## 📖 Scientific Abstract  

We propose an *adaptive quadratic integrate-and-fire* (**aQIF**) model with a phenomenological **slow ionic variable** to capture key features of neuronal excitability.  
Building on a previous three-variable extension of the *adaptive exponential integrate-and-fire* (**AdEx**) model, we reformulate it in **aQIF₍ᵢ₎** form to incorporate slow ionic regulation within a minimal framework.  

We first perform a **steady-state analysis** to characterize the model and its main parameters.  
Using **singular perturbation methods**, we then separate the dynamics into:
- a **fast subsystem** (*layer problem*), and  
- a **slow subsystem** (*reduced problem*),  

which enables a systematic investigation of **time-scale interactions**.

This approach reveals a broad repertoire of dynamical patterns:
> chaotic-like dynamics, fast spiking, bursting, doublet-like firing, canard-like events, and oscillations.

These results demonstrate the model’s ability to reproduce both **normal and pathological neuronal activity**.  
Beyond the single-neuron level, this formulation paves the way for **mean-field extensions** and offers new perspectives for modeling **spontaneous** or **central pattern generator (CPG)-like activity** without external input.

In particular, the parameter *Z₀* allows formalization of an **open system**, while focusing on the interplay between the three variables *(V, w, z)* and on the role of the **reset mechanism** along the slow manifold.

🔗 References: 
[1] Depannemaecker et al., bioRxiv, 2024 – https://doi.org/10.1101/2024.08.01.606188 

[2] Carlu et al., J. Neurophysiol., 2020 – https://doi.org/10.1152/jn.00399.2019

---

## ⚙️ Installation
```bash
git clone https://github.com/helenesoydemir/aQIFI-model.git
cd aQIFI-model
pip install -r requirements.txt

<!-- # Modeling and Mitigating Social Engineering Malware: Integrating Malware–Opinion Dynamics with Optimal Impulse Control Approaches -->

The code for the paper  
**"Modeling and Mitigating Social Engineering Malware: Integrating Malware–Opinion Dynamics with Optimal Impulse Control Approaches"**  


<!-- --- -->

<!-- ## Abstract
Social engineering malware, which exploits both technical and human vulnerabilities, presents challenges for individuals and organizations.  
Existing studies typically focus on either technical or human vulnerabilities in isolation, overlooking their coupled effects.  
This study introduces a **mathematical framework** that integrates:
1. a **coupled malware–opinion dynamics model** to capture the interaction between malware spread and human awareness, and  
2. an **optimal impulse control strategy** to mitigate social engineering malware.  

Theoretical analysis derives conditions for optimal impulse timing and intensity, and an iterative algorithm is developed to compute these strategies efficiently.  
Experiments conducted on **three real-world social networks** and **synthetic scale-free networks** demonstrate that our approach achieves an optimal balance between control cost and malware losses, emphasizing the value of **routine patching and awareness training** in cybersecurity resilience. -->


## Datasets

This repository includes or references four representative social network datasets used in the experiments:

| Dataset | Description | Source / Notes |
|----------|--------------|----------------|
| `email-univ` | University email communication network | Real-world dataset |
| `rt_assad` | Retweet (Twitter) network during a political event | Real-world dataset |
| `socfb-nips-ego` | Facebook friendship network (NIPS ego subset) | SNAP collection |
| `socfb-Simmons81` | Facebook social network (Simmons College) | SNAP collection |

These networks are used to evaluate the scalability and robustness of the proposed model across **different topological structures**.  
You may replace them with your own `.edges` files located in the `data/` directory.


## Set Up

contourpy==1.3.0
cycler==0.12.1
fonttools==4.54.1
igraph==0.11.8
kiwisolver==1.4.7
llvmlite==0.43.0
matplotlib==3.5.0
networkx==2.8.4
numba==0.60.0
numpy==1.26.4
packaging==24.1
pandas==2.2.3
pillow==11.0.0
pyparsing==3.2.0
python-dateutil==2.9.0.post0
pytz==2024.2
scipy==1.14.1
setuptools-scm==8.1.0
six==1.16.0
texttable==1.7.0
tomli==2.1.0
tzdata==2024.2


## How to Run the Code

<!-- 1. **Build the multiplex network**  
   - The function `create_multiplex_network_with_connected_nodes_edges()` in `network.py` constructs a coupled social–technical network.   -->

1. **Simulate malware–opinion dynamics**
   - Run `opinionMalware.py` to perform the **optimal control experiment**.  
   <!-- - Run `opinionMalwareRandom.py` and `opinionMalwareRandom_II.py` for **random baseline simulations**. -->

<!-- 3. **Output**
   - Results (infection level, awareness, control intensity, and payoff curves) are saved under the `result_data/` directory. -->

<!-- ---

## File Description

| File | Description |
|------|-------------|
| `network.py` | Builds and visualizes the coupled social and scale-free network. |
| `opinionMalware.py` | Main simulation of the optimal impulse control model. |
| `opinionMalwareRandom.py` | Randomized control strategy simulation. |
| `opinionMalwareRandom_II.py` | Partial random control with fixed parameters. |
| `result_data/` | Stores experiment results. | -->

<!-- --- -->




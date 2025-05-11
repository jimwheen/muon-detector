# Muon Detection Project
## Project Description
A muon detector designed for instructional use and data analysis, using inexpensive Geiger counter modules. By stacking two modules and narrowing their field of view, we can detect muons (high-energy cosmic particles capable of penetrating both counters)  through coincidence detection. The signal outputs are processed through a custom-built coincidence detection circuit.
## Background
During my first co-op at ASL Environmental Sciences, I gained experience working with time-series datasets and MATLAB. Inspired to continue this skill development, I began a personal project. A discussion with my father (a physics teacher) about how students struggle with understanding muons in special relativity led to the idea of building an affordable muon detector for his classroom.
## Pulse Width Optimization and Circuit Modifications
The stock Geiger counter modules output a 1 ms pulse, a wide window for coincidence detection which increases the chance of false positives and missed muon events. Since muons travel at nearly the speed of light, minimizing the time window is critical for accurate detection.
### Theoretical vs. Practical Analysis
From the module schematic, I identified a 555 timer in a monostable configuration, controlling the pulse width, as seen below:
![Pulse Width Circuit in Geiger Counter Module](pulse_circuit.png)

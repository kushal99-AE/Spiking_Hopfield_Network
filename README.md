# Spiking_Hopfield_Network
A spiking neural network implementation of the Hopfield Network using PyTorch and snnTorch. This project reconstructs original images from noisy inputs by leveraging biologically inspired Leaky Integrate-and-Fire (LIF) neurons and Hebbian learning principles. Tested across multiple datasets like Sklearn Images, MNIST, Fashion MNIST, and Road Signs

# Spiking Hopfield Network (SHN)
This repository implements a **Spiking Hopfield Network** (SHN) using PyTorch and snnTorch. SHN extends the classical Hopfield Network with spiking models like the **Leaky-Integrate-and-Fire (LIF)** neuron.

## **Project Summary**
The SHN reconstructs original images from noisy inputs across various datasets:
- **Sklearn Images**: Astronaut, Camera, Horse, Coffee
- **MNIST**: Handwritten digits
- **Fashion MNIST**: Clothing items
- **Road Signs**: Complex real-world images

Key components:
1. **Input Data Encoding**: Rate-based spike trains
2. **Neuron Model**: LIF Neurons for membrane potential dynamics
3. **Hebbian Learning**: Weight update based on "Cells that fire together, wire together"
4. **Output Spike Generation**: Recurrent feedback for pattern recall

---

## **Project Architecture**
![Architecture Diagram](docs/architecture.png) *(Placeholder for a diagram)*
<img width="975" alt="Screenshot 2024-12-16 at 8 23 27 PM" src="https://github.com/user-attachments/assets/8e87f435-5ea5-46b3-9029-825e9a754245" />

1. **Rate Encoding**: Convert images into spike trains over time steps.
2. **LIF Neurons**: Simulate neuron firing based on input spikes.
3. **Hebbian Learning**: Adjust weights to memorize patterns.
4. **Spike Generation**: Generate output spikes and iterate for reconstruction.

---

## **Performance Analysis**
- **Sklearn Images**: Handles simpler patterns but struggles with finer noise.
- **MNIST**: Struggles with complex handwritten digits.
- **Fashion MNIST**: Reasonable reconstruction of clothing patterns.
- **Road Signs**: Good recall performance on real-world patterns.

### Results Preview:
| Dataset         | Noise Level | Reconstruction Quality |
|-----------------|------------|-------------------------|
| Sklearn Images  | 30%        | Moderate               |
| MNIST           | 30%        | Limited                |
| Fashion MNIST   | 30%        | Reasonable             |
| Road Signs      | 30%        | Good                   |

---



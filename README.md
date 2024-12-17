# Spiking_Hopfield_Network
A spiking neural network implementation of the Hopfield Network using PyTorch and snnTorch. This project reconstructs original images from noisy inputs by leveraging biologically inspired Leaky Integrate-and-Fire (LIF) neurons and Hebbian learning principles. Tested across multiple datasets like Sklearn Images, MNIST, Fashion MNIST, and Road Signs


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

<img width="975" alt="Screenshot 2024-12-16 at 8 23 27 PM" src="https://github.com/user-attachments/assets/8e87f435-5ea5-46b3-9029-825e9a754245" />

The architecture consists of:

1. **Input Data Encoding:** Converts images into spike trains using rate encoding.
2. **Leaky Integrate-and-Fire Neurons:** Simulate neuron dynamics and membrane potentials.
3. **Hebbian Weight Update:** Updates weights based on neuron firing activity.
4. **Energy Minimization:** Network evolves towards stable patterns by minimizing energy.
5. **Output Spike Generation:** Final spiking activity recalls stored patterns.

---

## **Performance Analysis**
- **Sklearn Images**: Handles simpler patterns but struggles with finer noise.
- **MNIST**: Struggles with complex handwritten digits.
- **Fashion MNIST**: Reasonable reconstruction of clothing patterns.
- **Road Signs**: Good recall performance on real-world patterns.


---
## **Challenges**
1. Lack of online resources for integrating spiking dynamics into Hopfield Networks.
2. Debugging tensor operations and spiking behavior in PyTorch.
3. Visualizing neuron interactions and spike activity.

## **References**
1. Hopfield Network Is All You Need Paper - https://github.com/ml-jku/hopfield-layers.
2. takyamamoto/Hopfield-Network: Hopfield network implemented with Python (https://github.com/user-attachments/assets/b206ec31-faf3-4c8b-bad5-758383e5dfeb)
3. snnTorch Documentation - https://snntorch.readthedocs.io/en/latest/
4. PyTorch Documentation - https://pytorch.org/


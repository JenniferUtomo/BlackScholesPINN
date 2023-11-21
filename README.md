# BlackScholesPINN
Physics Informed Neural Network (PINN) is used to solve Black-Scholes PDE on European and American option. The model is used from Sifan et al. model in https://github.com/PredictiveIntelligenceLab/GradientPathologiesPINNs

There are several changes that I made in this code but I didn't change it there because it is only the combination of some activation functions and learning rate parameter
1. tanh becomes tf.keras.activations.swish or tf.keras.activations.selu or tf.keras.activations.gelu
2. self.adaptive_constant_ic_val and self.adaptive_constant_bc_val = np.array(1.0) becomes 0.1, 1.25, 1.5, and 2.0.

import numpy as np

def tanh(x):
    return np.tanh(x)

w1 = np.random.uniform(-0.5, 0.5)
w2 = np.random.uniform(-0.5, 0.5)
w3 = np.random.uniform(-0.5, 0.5)
w4 = np.random.uniform(-0.5, 0.5)

b1 = 0.5
b2 = 0.7

x1, x2 = 0.3, -0.2

h1 = tanh(w1 * x1 + w2 * x2 + b1)
h2 = tanh(w3 * x1 + w4 * x2 + b1)

w5 = np.random.uniform(-0.5, 0.5)
w6 = np.random.uniform(-0.5, 0.5)

output = tanh(w5 * h1 + w6 * h2 + b2)

# Print
print("Output of the network:", output)


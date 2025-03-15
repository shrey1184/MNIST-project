# MNIST-project
So, here is my first project on neural network Though it is not that great of a project, it surely made me learn different concepts and processes to create a neural network from scratch.
Here is the procedure that I followed to make this project
# Import
import libraries like pandas, numpy, and pyplot(from matplotlib) as pd, np, and plt, resp.
import dataset given in this repository

Our NN will have a simple two-layer architecture. Input layer  a[0]
  will have 784 units corresponding to the 784 pixels in each 28x28 input image. A hidden layer  a[1]
  will have 10 units with ReLU activation, and finally our output layer  a[2]
  will have 10 units corresponding to the ten digit classes with softmax activation.

# For Forward propagation
Z[1]=W[1]X+b[1]
A[1]=gReLU(Z[1])) (Use of ReLu - rectified linear unit)
Z[2]=W[2]A[1]+b[2]
A[2]=gsoftmax(Z[2])

# For Backward propagation
dZ[2]=A[2]−Y
dW[2]=1mdZ[2]A[1]T
dB[2]=1mΣdZ[2]
dZ[1]=W[2]TdZ[2].∗g[1]′(z[1])
dW[1]=1mdZ[1]A[0]T
dB[1]=1mΣdZ[1]

# To update parameters
W[2]:=W[2]−αdW[2]
b[2]:=b[2]−αdb[2]
W[1]:=W[1]−αdW[1]
b[1]:=b[1]−αdb[1]

# Test
Test prediction by changing the values in test_prediction()



Model: "MNISTExample"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 input_1 (InputLayer)        [(None, 28, 28, 1)]       0         
                                                                 
 conv1 (Conv2D)              (None, 28, 28, 32)        832       
                                                                 
 pool1 (MaxPooling2D)        (None, 14, 14, 32)        0         
                                                                 
 conv2 (Conv2D)              (None, 14, 14, 64)        51264     
                                                                 
 pool2 (MaxPooling2D)        (None, 7, 7, 64)          0         
                                                                 
 reshape (Reshape)           (None, 3136)              0         
                                                                 
 dense1 (Dense)              (None, 1024)              3212288   
                                                                 
 dense2 (Dense)              (None, 10)                10250     
                                                                 
 softmax (Softmax)           (None, 10)                0         
                                                                 
=================================================================
Total params: 3,274,634
Trainable params: 3,274,634
Non-trainable params: 0
_________________________________________________________________
Epoch 1/10

Epoch 2/10

Epoch 3/10

Epoch 4/10

Epoch 5/10

Epoch 6/10

Epoch 7/10

Epoch 8/10

Epoch 9/10

Epoch 10/10

94/94 - 0s - loss: 0.1546 - accuracy: 0.9460 - 162ms/epoch - 2ms/step
2022-07-18 14:45:19.643525, loss = 0.154644, accuracy = 0.946000
Parameter of the model:
conv1/kernel:0:	(5, 5, 1, 32)
conv1/bias:0:	(32,)
conv2/kernel:0:	(5, 5, 32, 64)
conv2/bias:0:	(64,)
dense1/kernel:0:	(3136, 1024)
dense1/bias:0:	(1024,)
dense2/kernel:0:	(1024, 10)
dense2/bias:0:	(10,)
Succeeded building model in TensorFlow2!
Succeeded building engine!
Binding0-> (-1, 1, 28, 28) (1, 1, 28, 28) DataType.FLOAT
Binding1-> (-1, 1) (1, 1) DataType.INT32
inputH0 : (1, 1, 28, 28)
outputH0: (1, 1)
[[8]]
Succeeded running model in TensorRT!
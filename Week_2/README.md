# EIP_Week_2

Group Members:
Sakthi Ganesh M - https://github.com/yasuo19/EIP4/tree/master/Week%202


Project Score: [0.019707133340882137, 0.9948]


Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 39s 647us/step - loss: 0.5228 - acc: 0.8541 - val_loss: 0.0858 - val_acc: 0.9842
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 13s 211us/step - loss: 0.2491 - acc: 0.9285 - val_loss: 0.0561 - val_acc: 0.9866
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 13s 209us/step - loss: 0.1959 - acc: 0.9425 - val_loss: 0.0452 - val_acc: 0.9874
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 13s 218us/step - loss: 0.1647 - acc: 0.9486 - val_loss: 0.0352 - val_acc: 0.9912
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 13s 211us/step - loss: 0.1497 - acc: 0.9507 - val_loss: 0.0359 - val_acc: 0.9907
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 13s 215us/step - loss: 0.1395 - acc: 0.9507 - val_loss: 0.0312 - val_acc: 0.9909
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 13s 216us/step - loss: 0.1297 - acc: 0.9524 - val_loss: 0.0266 - val_acc: 0.9926
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 13s 214us/step - loss: 0.1191 - acc: 0.9555 - val_loss: 0.0263 - val_acc: 0.9926
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 13s 211us/step - loss: 0.1174 - acc: 0.9543 - val_loss: 0.0242 - val_acc: 0.9927
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 13s 209us/step - loss: 0.1109 - acc: 0.9553 - val_loss: 0.0244 - val_acc: 0.9935
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 13s 210us/step - loss: 0.1083 - acc: 0.9564 - val_loss: 0.0210 - val_acc: 0.9937
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 13s 213us/step - loss: 0.1045 - acc: 0.9571 - val_loss: 0.0200 - val_acc: 0.9942
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 14s 226us/step - loss: 0.1041 - acc: 0.9556 - val_loss: 0.0228 - val_acc: 0.9944
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 13s 212us/step - loss: 0.0995 - acc: 0.9574 - val_loss: 0.0204 - val_acc: 0.9946
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 13s 209us/step - loss: 0.0991 - acc: 0.9569 - val_loss: 0.0198 - val_acc: 0.9942
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 13s 210us/step - loss: 0.0978 - acc: 0.9570 - val_loss: 0.0197 - val_acc: 0.9941
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 13s 209us/step - loss: 0.0938 - acc: 0.9582 - val_loss: 0.0203 - val_acc: 0.9942
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 13s 210us/step - loss: 0.0921 - acc: 0.9584 - val_loss: 0.0206 - val_acc: 0.9940
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 13s 211us/step - loss: 0.0932 - acc: 0.9576 - val_loss: 0.0215 - val_acc: 0.9938
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 13s 210us/step - loss: 0.0903 - acc: 0.9586 - val_loss: 0.0197 - val_acc: 0.9948
<keras.callbacks.History at 0x7f5a81f08cc0>







----------------------------------------------------------------------------------------------------------------

# Strategy

- In the initial time, we tried reducing the no of layers keeping in mind the kernel size be same as before, like 16, 32. But didn't get high accuracy. If we try to increase the kernel size, the no of parameters would sky-rocket.
Also, if to accomoddate more number of higher kernel size to restrict no of parameters, if we try to reduce no of layers, the accuracy went down.

- So, we tried to restict the kernel size to 10, 16 and increase the no on layers if necessary, for the number of parameters not to exceed 15,000 and get the desired result, which we acheived.

- Also, in notebook 8, 1x1 convolution was done before maxpooling, we moved it after maxpooling. 



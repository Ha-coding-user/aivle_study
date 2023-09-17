Image Deep Learning

1. Not MNIST Data
   - Data : !wget http://yaroslavvb.com/upload/notMNIST/notMNIST_small.mat
   - model
     - Input
     - Flatten
     - Dense(256, activaion='relu')
     - Dense(256, activaion='relu')
     - BatchNormalizaion
     - Dropout : 0.2
     - Dense(128, activaion='relu')
     - Dense(128, activaion='relu')
     - BatchNormalization
     - Dropout : 0.2
     - Dense(64, activation='relu')
     - Dense(64, activation='relu')
     - BatchNormalizaion
     - Dropout
     - Output
  - Compile
     - optimizer : adam
     - loss : categorical_crossentropy

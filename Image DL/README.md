Image Deep Learning

1.1 Not MNIST Data
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

1.2 My_First_CNN
   - Data : tensorflow.keras.datasets -> MNIST Data
   - Model
     - Input
     - Conv2D : filters=128, kernel_size=(3,3, strides=1, padding='same', acitvation='relu'
     - Conv2D : filters=128, kernel_size=(3,3, strides=1, padding='same', acitvation='relu'
     - MaxPool2D : pool_size=(2,2)
     - Conv2D : filters=64, kernel_size=(3,3, strides=1, padding='same', acitvation='relu'
     - Conv2D : filters=64, kernel_size=(3,3, strides=1, padding='same', acitvation='relu'
     - MaxPool2D : pool_size=(2,2)
     - Flatten
     - Dense : 128, activation='relu'
     - Output
   - Compile
     - optimizer : adam
     - loss : categorical_crossentropy
   - Accuracy
     - Train : 99.25%
     - Test : 98.97%

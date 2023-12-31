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
    
1.3 CNN_exercise 1
   - Data : tensorflow.keras.datasets -> fashion_MNIST
   - Model
     - Input
     - Conv2D : filters=32, kernel_size=(3,3), padding=same, activation=relu
     - BatchNormalization
     - Conv2D : filters=32, kernel_size=(3,3), padding=same, activation=relu
     - BatchNormalization
     - MaxPool2D : pool_size=(2,2), strides=(2,2)
     - Dropout : 0.25
     - Conv2D : filters=64, kernel_size=(3,3), padding=same, activation=relu
     - BatchNormalization
     - Conv2D : filtesr=64, kernel_size=(3,3), padding=same, activation=relu
     - BatchNormalization
     - MaxPool2D : pool_size=(2,2), strides=(2,2)
     - Dropout : 0.25
     - Flatten
     - Dense : 512, activation=relu
     - BatchNormalization
     - Output
   - Compile
     - optimizer : adam
     - loss : categorical_crossentropy
   - Accuracy
     - Train : 96.87%
     - Test : 92.63%

1.4 CNN_exercise 2
   - Data : tensorflow.keras.datasets -> CIFAR10
   - Model
     - Input
     - Conv2D : filters=32, kernel_size=(3,3), padding=same, activation=relu
     - Conv2D : filters=32, kernel_size=(3,3), padding=same, activation=relu
     - BatchNormalization
     - MaxPool2D : pool_size=(2,2), strides=(2,2)
     - Dropout : 0.25
     - Conv2D : filters=64, kernel_size=(3,3), padding=same, activation=relu
     - Conv2D : filters=64, kernel_size=(3,3), padding=same, activation=relu
     - BatchNormalization
     - MaxPool2D : pool_size=(2,2), strides=(2,2)
     - Dropout : 0.25
     - Flatten
     - Dense : 1024, activation=relu
     - BatchNormalization
     - Dropout : 0.35
     - Output
   - Compile
     - optimizer : adam
     - loss : categorical_crossentropy
   - Accuracy
     - Train : 92.14%
     - Test : 79.27%

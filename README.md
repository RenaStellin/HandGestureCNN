# Hand Gesture Identification Using Proposed Convolution Neural Network Model

## Dataset created by me
![](RenaHandGesture.png)

## Proposed Convolution Neural Network ALgorithm

Proposed CNN Algorithm:

learning rate <- 0.01

weights, biases <- random

train-test split <- 0.8:0.2

epoch <- 10

batch_size <- 128

batches_count <- train_data / batch_size

while epoch >= 1 do

  while batches_count >= 1 do 
  
      Convolution2D (64, (3, 3))
      
      Convolution2D (64, (3, 3))
      
      MaxPooling2D ()
      
      Dropout (0.2)
      
      Convolution2D (128, (3, 3))
      
      Convolution2D (128, (3, 3))
      
      Flatten ()
      
      Dense (512, ‘relu’)
      
      Dropout (0.2)
      
      predicted_class <- Dense (10, ‘softmax’)
      
      error <- Loss (predicted_class, actual_class)
      
      BackPropagation (error) #Updates weights and biases
      
      batches_count  batches_count – 1
      
   end while
   
   epoch <- epoch - 1
   
end while 

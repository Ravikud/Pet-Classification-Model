# Pet-Classification-Model
It is a deep learning model to find whether the images belongs to cat or dog.

Classification of images between two class cat and dog using CNN with image augmentation .
We are using image augmentation to increase the amount of training data using augmentation by using from keras.preprocessing.image import ImageDataGenerator.

Accuracy we achieved : 100 % percent accuracy by CNN Model with epoch 13th and  val_loss of 0.3049.

Data is very limited and costly in some cases such as medical imagery. To get the best out of it , we are using ImageDataGenerator and creating multiple images for each image we have in our training data set by rotation ,zoom in 
datagen = ImageDataGenerator( rotation_range=40, width_shift_range=0.2, height_shift_range=0.2, rescale=1./255, shear_range=0.2, zoom_range=0.2, horizontal_flip=True, fill_mode='nearest')

For details , read Documentation :http://keras.io/preprocessing/image/
It uses data that can be downloaded at: https://www.kaggle.com/c/dogs-vs-cats/data.
In our setup, we:
•	created a Projects folder
•	created train/ and validation/ subfolders inside Projects folder 
•	created cats/ and dogs/ subfolders inside train/ and validation


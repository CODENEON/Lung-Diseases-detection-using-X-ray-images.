# Lung-Diseases-detection-using-X-ray-images.
using CNN and Transfer Learning to classify diseases from X-ray images

STEPS TO RUN THE CODE.

1.	First download anaconda distribution if you don't have by visiting https://www.anaconda.com/products/individual
2.	Install all the necessary libraries and frameworks from anaconda dashboard environment section( tensorflow, mtaplotlib, glob, numpy )
3.	third install jupyter notebook on anaconda and then launch it.
4.	run pwd in jupyter notebook and know your current working directory and then create a folder called chest_xray in your current working directory, then download chest_xray(PNEUMONIA) dataset from kaggle--->https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
5.	Then extract the data zip in chest_xray folder that you previously created(your now have three folders test,train and val and each folder have 2 subfolders NORMAL AND PNEUMONIA
6.	After that download another Atelectasis dataset from kaggle NIH chest_ray dataset------->https://www.kaggle.com/nih-chest-xrays/data?select=images_001
7.	Again extract the zip in your chest_xray folder, then your'll get a new folder probably names images-001, after that create new folder called ATELECTASIS IN each test train and val directories.
8.	Go to newly created images_001 folder and cut 40 images and paste them in ATELECTASIS folder in val directory, again go to images_001 folder and then cut around 20% images and paste them in ATELECTASIS FOLDER IN test directory, then cut paste remaining images in ATELECTASIS FOLDER IN train directory.
9.	Your dataset is now prepared. 
10.  Now run each code column in jupyter notebook one by one, training the model will take some time when you run ( model.fit ) so have some patience, when your reach the end of the code on line 87 run model performance function, pass path of any image from val directory. Select either 0 or 1 or 2 to predict the result for passed image.
11.  0 is for running simple model made by us, 1 is for running       VGG16 model, 2 is for running InceptionV3 model.
12.  Compare which model give accurate predictions and conclude the project.

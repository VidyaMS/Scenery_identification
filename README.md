# Scenery_identification
This repo is for identification of scenery images such as mountains, glaciers, streets, buildings , sea and forest.   
Data source : https://www.kaggle.com/puneet6060/intel-image-classification.  
This analysis was done on Kaggle as computation with GPU was possible to expedite the working of CNN.  
  
Various diverse set of images of above given types has  been collected and made available in Kaggle datasets.   
Problem statement:  
Given the set of images, can we build a classifier to accurately identify the types of images?  
  
Using tensorflow the analysis is done by building various deep learning models.  
. The complexity of the model is increased slowly by adding new layers of CNN and MaxPooling.  
Once the model architecture that gives the maximum accuracy is identified, the hyperparameters such as learning rate and regularization technique of varying the drop rate was tested for test set accuracy.  
. An attempt to use transfer learning by using one of the pre trained model weights such as VGG16 is tested for test set accuracy.    

Conclusion.  
. Test set accuracy given by 7 layer CNN + Maxpooling model with 25 epochs is @0.85. We get the same accuracy by using transfer learning with VGG16 and 15 epochs.  
Augmentation techniques such as RandomFlip, RandomRotation and RandomZppm does not increase the test set accuracy beyond 0.85.  



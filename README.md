# Pneumonia-prediction-with-CNN-
## Key components of the project include:     
*  1. Image preprocessing: resizing, grayscale conversion, and augmentation. 
* 2. Model building: CNN architecture with layers like convolutional, pooling, 
dropout, and dense layers. 
* 3. Data Augmentation: Enhancing the training data using techniques like 
rotation, shifting, and flipping. 
* 4. Class Weights: Balancing the dataset by computing class weights to 
address the imbalance between pneumonia and normal images. 
* 5. Model training and evaluation: Using training, validation, and test datasets 
to train and evaluate the model’s performance. 

### the dataset used is a collection of chest X-rays which includes two directories: 
PNEUMONIA and NORMAL
## Data Preprocessing and Visualization - Data Extraction 
* First, we extract the dataset from a zip file and navigate to the dataset                              
directory  - Loading and Preparing the Data

## model building - CNN Model Architecture 
* We begin by building a basic CNN model to classify the X-ray images.   
The  architecture includes: 
* 1. Conv2D: Convolutional layers for feature extraction. 
* 2. MaxPooling2D: Pooling layers to reduce spatial dimensions. 
* 3. Flatten: To flatten the 2D feature maps into a 1D vector. 
* 4. Dense: Fully connected layers for classification. 
* 5. Dropout: To prevent overfitting by randomly dropping units during   
* training. - Model Training 
The model is then trained using the fit() function, where training data is 
passed along with validation data - Early Stopping and Class Weights 
To prevent overfitting and handle class imbalances, we use the following  
### techniques: 
* 1. Early Stopping: Monitors the validation loss to stop training when no 
improvement is observed. 
* 2. Class Weights: Compute the class weights using 
compute_class_weight() to address class imbalances between 
PNEUMONIA and NORMAL. 
## Data Augmentation and Final Model Training - Data Augmentation 
* To further improve the model’s robustness, we use ImageDataGenerator    
  to augment the training data. This includes transformations like rotation,   
  shifting, and flipping - Model Compilation and Training with Augmentation 
* The model is then compiled and trained using the augmented data 
* This ensures that the model trains on a variety of transformations,  
improving generalization.

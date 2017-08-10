[//]: # (Image References)

[image1]: ./images/wbc_cells.jpg "white blood cells"
[image2]: ./images/SigTuple_data/Test_Data/D0F6DE661D63.jpg "test"
[image3]: ./images/SigTuple_data/Submission_Data/D0F6DE661D63-mask.jpg "predicted_mask"

# White Blood Cells Segmentation (Udacity Machine Learning Capstone)

## Project Overview
White blood cells (also known as WBC or leukocytes) help our body fight infections by attacking bacteria, viruses and other germs that invade the body. A count of leukocytes can help reveal several hidden and undiagnosed diseases. In a manual microscopic review of blood samples, pathologists minutely examine the count and morphology (i.e. size and shape) of white blood cells.

Red blood cells (or RBC, or erythrocytes) are the most common type of blood cells, and they outnumber WBCs by about 600:1. So, in an image of a blood sample, you will see mostly RBCs,
with a few WBCs thrown in here and there.

![white blood cells][image1]

In manual process pathologists analyze the blood sample and count the WBC (white blood cells), but this is not accurately defined the correct count and related disease, they use predefined approach to determine the health of the person. But if we use Image segmentation using deep learning supervised algorithm model, it accurately demarcates the boundary of WBC
even when they are touching each other and identify correct count. This will improve the accuracy and speed of testing and yield better results.

__Developed an efficient Deep Learning model using CNN (Convolutional Neural Networks) to accurately demarcate the boundary of white blood cells in microscopic images of blood__
- Technologies used : Tensorflow, Keras, AWS

## File Structure of the project:

* The data set is present in __SigTuple_data__ folder. Training data is in __SigTuple_data/Train_Data__, after modified extra large images in train data, the new data files set is stored in __SigTuple_data/New_Train_Data__, Test data is in __SigTuple_data/Test_Data__ and predicted masks for test data is in __Submission_Data folder__.
* All the parameters including epochs, img dimensions and extra parameters are all stored in __all_params.py__ file
* Model is stored in __model.py__ file
* All the preprocessing and training and predicting masks are done using Jupyter notebook named __wbc_segmentation.ipynb__
* __capstone_project_report.pdf__ file describes the project architecture and implementation details
* __wbc_segmentation.pdf__ and .html files for representation purpose for jupyter notebook

__Please see the Jupyter notebook wbc_segmentation.ipynb for instructions to running the project.

Please find below images, the model returned after predicting masks for the test set.

![test][image2]
![predicted_mask][image3]

The first image showing the test image with white blood cells (blue area) and red blood cells (whitearea) cells. The second image showing predicted mask with white blood cells (white area).
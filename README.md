# White Blood Cells Segmentation (Udacity Machine Learning Capstone)

## Project Overview
White blood cells (also known as WBC or leukocytes) help our body fight infections by attacking bacteria, viruses and other germs that invade the body. A count of leukocytes can help reveal several hidden and undiagnosed diseases. In a manual microscopic review of blood samples, pathologists minutely examine the count and morphology (i.e. size and shape) of white blood cells.

Red blood cells (or RBC, or erythrocytes) are the most common type of blood cells, and they outnumber WBCs by about 600:1. So, in an image of a blood sample, you will see mostly RBCs,
with a few WBCs thrown in here and there.

![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/images/wbc_cells.jpg)

In manual process pathologists analyze the blood sample and count the WBC (white blood cells), but this is not accurately defined the correct count and related disease, they use predefined approach to determine the health of the person. But if we use Image segmentation using deep learning supervised algorithm model, it accurately demarcates the boundary of WBC
even when they are touching each other and identify correct count. This will improve the accuracy and speed of testing and yield better results.

Developed an efficient Deep Learning model using CNN (Convolutional Neural Networks) to accurately demarcate the boundary of white blood cells in microscopic images of blood
- Technologies used : Tensorflow, Keras, AWS

File Structure of the project:

* The data set is present in SigTuple_data folder. Training data is in SigTuple_data/Train_Data, after modified extra large images in train data, the new data files set is stored in SigTuple_data/New_Train_Data, Test data is in SigTuple_data/Test_Data and predicted masks for test data is in Submission_Data folder.
* All the parameters including epochs, img dimensions and extra parameters are all stored in all_params file
* Model is stored in model file
* All the preprocessing and training and predicting masks are done using Jupyter notebook named wbc_segmentation.ipynb
* capstone_project_report file describes the project architecture and implementation details
* wbc_segmentation.pdf and .html files for representation purpose for jupyter notebook

Please see the Jupyter notebook for complete running of the project.

Predicted masks for the test set:

![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/SigTuple_data/Test_Data/F1BFEA74B33D.jpg)
![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/SigTuple_data/Submission_Data/F1BFEA74B33D-mask.jpg)
![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/SigTuple_data/Test_Data/D28CDF85BDA3.jpg)
![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/SigTuple_data/Submission_Data/D28CDF85BDA3-mask.jpg)
![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/SigTuple_data/Test_Data/D0F6DE661D63.jpg)
![alt text](https://github.com/gottipati/wbc_segmentation/tree/master/SigTuple_data/Submission_Data/D0F6DE661D63-mask.jpg)

the first image showing the test image with white (blue area) and red (whitearea) cells. The second image is predicted mask with white blood cells (white area).
Libraries:
- Keras
- sklearn
- numpy
- matplotlib.pyplot
- pandas
- glob
- seaborn
- os
- csv
- PIL
- pydot

## PLEASE CHANGE PATH WHERE NEEDED !!!

Setup:
1) download and place the dataset following the dataset section of this README
2) change the paths of files where needed in the codes
3) if you need extra helping tools, they are available in the Helper Tool folder
4) Read the Report as it explains in depth the codes and their usage

Code:
My code works if placed all in one folder as seen in the folder named " All Codes and files in one folder"

DataSet:
Download the dataset from https://www.kaggle.com/jutrera/stanford-car-dataset-by-classes-folder
Place the folders of the dataset in the folder named "My_Cars"
The "train" folder should include the raw and uncropped pictures from the dataset
If you wish to crop, I have provided a tool to crop the images using the bounding boxes available in anno_train.csv just adjust the path for train folder, trainCropped and "anno_train.csv" inside the code named "Car_Extractor.ipynb" in the Helper Tools

What does each folder mean?:
- All Codes and files in one folder = a folder if you wish not to change the path of any of the codes
## Folder inside All Codes and files in one folder are left empty to save up space as the models are too big, use the models in the main folder####

- All Trial codes = includes all the attempts and the journey of to reach the final code, really helpful for the refinment process in the report

-Final Codes = two code files, one for the final architecture and one for the final pretrained model

- Helper Tools = contains 3 code files, Car_Extractor to crop the training images, Model_Summary to check the summary of each model and TestingTheModel a code to generate test score for the models with test dataset, StdAndMeanForAClass generates mean and std for each class but after changing the path.

- History_accuracy = was used to record the accuracy results (from fit_generator) as I didn't keep the codes before that, these are the first 13 results for the first 13 models. the names explain the evolution and difference of a model from previous models.

- My_Cars = folder contains empty folder but shows how to install tyhe dataset

- RandomSearchResults = contains the results of grid search, however the name was kept as I forgot to change it in the code

- RandomSearchResults with regularization = same as above with grid search however with regularization added

- Saved_Models = the most important folder, it contains the best models from each code from the "All Trial codes", the models can be called and seen using "Model_Summary" from the Helper Tools folder, you can visualize the accuracy of each model using "TestingTheModel" from the Helper Tools folder. a txt file will be found at the end of the folder named "Which model represents what" it explains the evolution of some of the models used.
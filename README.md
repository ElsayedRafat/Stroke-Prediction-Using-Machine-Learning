# Stroke-Prediction-Using-Machine-Learning
The aims of this project were to find apply machine learning models for predicting the stroke with different chosen features to identify everyone’s risk of stroke. Develop and evaluate ensemble model combining all the used models to identify risk of stroke. 
### Dataset
The data used in this project are available online in educational purpose use. The dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relevant information about the patient. The dataset provides 11 features and output column with a small percentage of missing values and reasonable number of features and data. The number of people have a risk of stroke is 498 and the 498 have no risk (after balancing the dataset). 
![Workflow](https://user-images.githubusercontent.com/56036913/152394361-ed993fae-b86a-4879-8816-e59b6779043e.PNG)
### Preprocessing
- Missing values
- Categorical data
- Feature scaling
### Data Splitting
First the dataset is split into two sets one for input which contains all the columns excluding (‘id’ and ‘stroke’) and the other set contains ‘stoke’ column only for the output. Then both sets subdivided into three smaller sets (training, validation, and testing). Both input and output sets split into 20% of the data for testing and the other 80% of the data split into 25% for validation and 75% for training
### MODELS
The proposed strategy focuses on machine learning procedures for stroke prediction, thus overcoming existing problems. Different machine learning methods may not perform equally a same feature set. By utilizing decision tree classifier, logistic regression classifier, C-support vector classifier random forest and voting classifier. COLAB used to develop the proposed system. The dataset is given as the input which is pre-processed to remove unwanted rows and columns to produce modified dataset, then the machine learning all algorithms are applied then compared and the most accurate model.
- Decision tree classifier
![DT](https://user-images.githubusercontent.com/56036913/152395826-e2450a34-a0b5-426d-a6ed-db18037314f8.PNG)
- C-support vector classifier
![C-support vector classifier](https://user-images.githubusercontent.com/56036913/152396283-0e9d40f8-b4a2-4856-b7d2-27105554e6f7.PNG)
- Random forest classifier
![RF](https://user-images.githubusercontent.com/56036913/152396479-507e1788-03a5-46c3-83bd-23d3a5e38b00.PNG)
- Voting classifier (Hard)
![HV](https://user-images.githubusercontent.com/56036913/152396821-f82a5070-9dc5-4217-a5e3-aeda455d0e70.PNG)
The classifier reached 81.6176 % accuracy of the training set and 80.2198% accuracy of the validation set.
- Voting classifier (soft)
The new soft voting classifier achieves over 83.4559% accuracy on the training set and 78.022% accuracy on the validation set.
### Results
After observation of all the models and the accuracy for each individual model after applying each on both training and validation set all the results shown on the table. 
![Results](https://user-images.githubusercontent.com/56036913/152397302-7f5d1272-3732-4f9a-ab67-bc6f76012456.PNG)
![Models](https://user-images.githubusercontent.com/56036913/152397437-d077abf2-ea6e-4dae-918d-8c64f72601ab.PNG)
Random forest classifier achieved the best results on both training and classification sets. Against all the odds the voting classifiers did not achieve the best results. Surprisingly, soft voting classifier achieved the worst accuracy in comparison with the other models. Hard voting classifier achieved the second-best accuracy in the validation set. Decision tree classifier achieved the achieved the second-best accuracy on the training set.
### Performace
![CM](https://user-images.githubusercontent.com/56036913/152397830-8f52c1b4-9c97-4d1c-9096-d51bb793454d.PNG)
![ROC](https://user-images.githubusercontent.com/56036913/152397961-d9a80f73-25d0-4d43-95d6-860125013c5d.PNG)



# Chest X-ray Classification Using CNN
Detect COVID-19 and Pneumonia using Chest X-ray and Convolutional Neural Network

The recent outbreak of Coronavirus Disease, COVID-19 has caused millions dealth globally since the occurence in early 2020. Besides COVID-19, another respiratory disease which has high mortality rate is pneumonia. In 2017, Pneumonia has taken more than 808,000 lives of children under age 5. These diseases share the similarity which affects the lung structure and disrupts the entire respiratory system. Therefore, early detection with high accuracy is crucial to enable early treatment be given. 

This study explored on the performance of three variations of Convolutional Neural Network (CNN) model: standard CNN, Separable CNN and Grouped CNN in classifying chest-X-ray to normal, COVID-19 and viral pneumonia classes. 

### Challenges
The differences between a normal lung and diseased lung on Chest X-ray can be spotted by an experienced medical expert easily.
![image](https://github.com/suetteh/Chest-X-ray-Classification/assets/65590665/e0efd930-3be2-49a2-94bd-5651a2cba068) 
![image](https://github.com/suetteh/Chest-X-ray-Classification/assets/65590665/0e4045a0-f0e8-41e4-b2c6-4e56181ce183)
Figure 1 Chest X-ray Images of normal lung (left) and lung opacity (right) (Fuat, 2023 )


### Library Utilized

### Data Source
The dataset used in this study is from the COVID-19 Chest X-ray Database from https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database. This database was created by a team of researchers from Qatar University (Doha, Qatar) and the University of Dhaka (Bangladesh) in collaboration with medical doctors from Pakistan and Malaysia.

### Data Preprocessing
Data pre-processing technique applied including cropping image to remove noises, data augmentation on class pneumonia training data to ensure equal amount of data is available tor training in all classes. Each base model was evaluated by comparing the accuracy and loss of training and validation data. Regularization was then performed to each base model to resolve overfitting and evaluated on test data. Metrics used for model performance evaluations include accuracy, loss, AUC, precision, recall and f1-score.

### Results/ Visualization
The results of the [standard CNN](https://github.com/suetteh/CXR-CNN/blob/main/Standard%20CNN.pdf), [separable CNN](https://github.com/suetteh/CXR-CNN/blob/main/Separable%20CNN.pdf), and [grouped CNN](https://github.com/suetteh/CXR-CNN/blob/main/Grouped%20CNN.pdf) are as presented in the attached files. Based on the [model performance comparison](https://github.com/suetteh/CXR-CNN/blob/main/Model%20Performance%20Comparison.pdf), further tuning was performed on the [best model](https://github.com/suetteh/CXR-CNN/blob/main/Tuning%20of%20Best%20Model.pdf) to improve the model performance.

### Possible Improvement


### Concolusion:
Separable CNN showed the best performance, 89.36% accuracy, 0.3071 loss, 0.9704 AUC, macro average 0.89 precision, 0.9 recall and 0.9 f1-score.

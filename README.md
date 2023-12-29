# Chest X-ray Classification Using CNN
Detect COVID-19 and Pneumonia using Chest X-ray and Convolutional Neural Network

The recent outbreak of Coronavirus Disease, COVID-19 and pneumonia, the disease which cost 808,000 lives of children under age 5 have been witnessed to affect the lung structure which in turn disrupt0ing the entire respiratory system. Therefore, early detection with high accuracy enables treatment to be given early to keep the condition under controlled.

This study explored on the performance of three variations of simple CNN model, standard CNN, Separable CNN and Grouped CNN in classifying chest-X-ray to normal, COVID-19 and viral pneumonia classes. 

Dataset preparation:
The dataset used in this study is from the COVID-19 Chest X-ray Database from https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database. This database was created by a team of researchers from Qatar University (Doha, Qatar) and the University of Dhaka (Bangladesh) in collaboration with medical doctors from Pakistan and Malaysia.

Data pre-processing technique applied including cropping image to remove noises, data augmentation on class pneumonia training data to ensure equal amount of data is available tor training in all classes. Each base model was evaluated by comparing the accuracy and loss of training and validation data. Regularization was then performed to each base model to resolve overfitting and evaluated on test data. Metrics used for model performance evaluations include accuracy, loss, AUC, precision, recall and f1-score.

Model Performance: The results of the [standard CNN](https://github.com/suetteh/CXR-CNN/blob/main/Standard%20CNN.pdf), [separable CNN](https://github.com/suetteh/CXR-CNN/blob/main/Separable%20CNN.pdf), and [grouped CNN](https://github.com/suetteh/CXR-CNN/blob/main/Grouped%20CNN.pdf) are as presented in the attached files. Based on the [model performance comparison](), further tuning was performed on the [best model]() to improve the model performance.

Concolusion:
Separable CNN showed the best performance, 89.36% accuracy, 0.3071 loss, 0.9704 AUC, macro average 0.89 precision, 0.9 recall and 0.9 f1-score.

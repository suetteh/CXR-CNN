# Chest X-ray Classification Using CNN
Detect COVID-19 and Pneumonia using Chest X-ray and Convolutional Neural Network

The recent outbreak of Coronavirus Disease, COVID-19 and pneumonia, the disease which cost 808,000 lives of children under age 5 have been witnessed to affect the lung structure which in turn disrupting the entire respiratory system. Therefore, early detection with high accuracy enables treatment to be given early to keep the condition under controlled.

This study explored on the performance of three variations of simple CNN model, standard CNN, Separable CNN and Grouped CNN in classifying chest-X-ray to normal, COVID-19 and viral pneumonia classes. Data pre-processing technique applied including cropping image to remove noises, data augmentation on class pneumonia training data to ensure equal amount of data is available tor training in all classes. Each base model was evaluated by comparing the accuracy and loss of training and validation data. Regularization was then performed to each base model to resolve overfitting and evaluated on test data. Metrics used for model performance evaluations include accuracy, loss, AUC, precision, recall and f1-score.

Concolusion:
Separable CNN showed the best performance, 89.36% accuracy, 0.3071 loss, 0.9704 AUC, macro average 0.89 precision, 0.9 recall and 0.9 f1-score.

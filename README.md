# Chest X-ray Classification Using Variations of CNN Models

The recent outbreak of Coronavirus Disease, COVID-19 has caused millions dealth globally since the occurence in early 2020. Besides COVID-19, penumonia is also a known respiratory disease with high mortality rate. In 2017, pneumonia has taken more than 808,000 lives of children under age 5. These diseases share the similarity which is that they affect the lung structure causing the disruptions of the entire respiratory system. Therefore, early detection with high accuracy is crucial to enable early treatment be given. 

This study explored on the performance of three variations of Convolutional Neural Network (CNN) models: standard CNN, Separable CNN and Grouped CNN in classifying chest-X-ray to normal, COVID-19 and viral pneumonia classes.  

### Challenges
It was observed that after training the models for 30 epochs respectively, the base models achieved 100% accuracy. However, these models failed to generalize on unseen data, presented an overfitting characteristic. Regularization techniques including dropout and batch normalization were applied to overcome this issue. 

### Tools Utilized
This project was completed using python.
Computer vision and image processing techniques were applied in this project.
library: keras, tensorflow, numpy, matplotlib, seaborn, imageio, cv2

### Data Source
The dataset used in this study is from the [COVID-19 Chest X-ray Database] (https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database). This database was created by a team of researchers from Qatar University (Doha, Qatar) and the University of Dhaka (Bangladesh) in collaboration with medical doctors from Pakistan and Malaysia.

### Data Preprocessing
Data pre-processing technique applied include cropping image to remove noises, data augmentation on class pneumonia training data to ensure equal amount of data is available tor training in all classes. Each base model was evaluated by comparing the accuracy and loss of training and validation data. Regularization was then performed to each base model to resolve overfitting and evaluated on test data. Metrics used for model performance evaluations include accuracy, loss, AUC, precision, recall and f1-score.

### Results Evaluation
To evaluate the fitness of model, the accuracy, loss and AUC of each model was compared between the training and validation data. Furthermore, upon model applying regularization technique on the base model, [the macro average precision, recall and f1-score were then evaluated on the test data](https://github.com/suetteh/Chest-X-ray-Classification/blob/main/Model%20Performance%20Comparison.pdf). 

### Possible Improvement
Based on the model performance on test data, it is observed that the models struggle to differentiate normal and COVID-19 CXR. Thus, additional preprocessing step such as heatmap generation on CXR could be performed before feeding the images to the model. By highlighting the lung structure, the difference in pixels could be more vivid for the model to detect. 

![image](https://github.com/suetteh/Chest-X-ray-Classification/assets/65590665/5b9a67ee-5145-4f8e-a56c-d9ab72cc2962)

figure: Sample final heatmaps of COVID-19 CXR with confidence scores (Kusakunniran, 2021).

### Concolusion:
The results of the [standard CNN](https://github.com/suetteh/CXR-CNN/blob/main/Standard%20CNN.pdf), [separable CNN](https://github.com/suetteh/CXR-CNN/blob/main/Separable%20CNN.pdf), and [grouped CNN](https://github.com/suetteh/CXR-CNN/blob/main/Grouped%20CNN.pdf) are as presented in the attached files. Based on the [model performance comparison](https://github.com/suetteh/CXR-CNN/blob/main/Model%20Performance%20Comparison.pdf), further tuning was performed on the [best model](https://github.com/suetteh/CXR-CNN/blob/main/Tuning%20of%20Best%20Model.pdf) to improve the model performance.
In concolusion, Separable CNN showed the best performance, 89.36% accuracy, 0.3071 loss, 0.9704 AUC, macro average 0.89 precision, 0.9 recall and 0.9 f1-score.

### Reference:
Kusakunniran, W. K. (2021). COVID-19 detection and heatmap generation in chest x-ray images. J Med Imaging (Bellingham).


# Digit_Recognizer
 

**Goal:** <br>

Recognize hand written digits' images (32x32 pixels in grey scale) and predict the labels which are from 0 to 9. 
It's also an ongoing competition. <br> 
Kaggle link: https://www.kaggle.com/c/digit-recognizer

**Dataset:** <br>

The dataset is obtained from the link above <br>
- Training dataset: 42,000 images, labeled 
- Test dataset: 28,000, unlabeled

Since we do not have labels for the test set we create a test set from the training set (20% of training set, technically validation set) and tabulate the results

<br>
    
**Key takeaways:** <br>

- Following are results on the test dataset 

| Model | Test Set Accuracy |
| :-: | :-: |
| Logistic Regression | 0.92 |
| Shallow Neural Network | 0.89 | 
| Fully Connected Neural Network  | 0.94 |
| Optimized Fully Connected Neural Network | 0.97 | 
| CNN architecture | 0.99|

- Logistic Regression serves as the baseline for all the models


- Neural Networks with more than 2 hidden layers performs well on this dataset. The optimized Fully Connected Neural Network Architechture has 3 Hidden layers of 128 nodes and Dropout Regularization


- Convolutional Neural Network Architechture performs exceptionally well on the dataset. The Architecture is inspired from LeNet-5 architecture. It has 2 Convolution Layers (filter size - 3x3), 2 Fully Connected layers (128, 64 nodes) and Dropout Regularization <br>

**Kaggle Submission Result:** Accuracy = 0.989 (Top 40 percentile) on unlabeled dataset


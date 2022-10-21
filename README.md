**Classification of COVID-19 from Chest X-ray images via  Convolutional Neural Network**

**Introduction**

COVID-19 is a rapidly spreading viral disease that can cause serious lung inflammation and 
even death. Many studies have shown that chest radiography images are highly suitable for 
differentiating patients with chronic diseases from those with normal healthy lungs. 
Chest X-ray is used for this project having taken into consideration its wider applicability, driven by 
factors such as the substantially lower cost and far shorter acquisition time, compared to CT 
scans. With advances in the field of artificial intelligence including Convolutional Neural 
Networks (CNN), it has become possible to apply sophisticated computer analysis to medical 
images and trials have proven this approach with reassuringly high success rates. 

**Methodology**

This paper proposes to develop a Convolutional Neural Networks to distinguish COVID-19 chest X-ray 
images. Two distinct CNN models were developed for the binary classification of COVID-19 
from Normal or Lung opacity cases by examination of their accuracies and errors in order to 
determine the best model. The first model was named CNN2021 (7 layers) which was 
developed from scratch and the second was named as TFVGG16 (15 layers) built by using 
state-of-the-art transfer learning techniques from machine learning. These models were 
experimented on 3 distinct datasets (sample sizes ranging from 2,500 to 13,000), each having 
two classes of data (COVID-19 and non-COVID-19). Dataset sample images were randomly 
selected in an initial “data splitting” stage as follows: 0.70 training set, 0.15 validation set and 
0.15 test set. The images were then passed through a pre-processing stage to standardise all the 
images to a size of 224 by 224 pixels greyscale before being used for training the two models. 
Both models were trained with the training data and later tested on the test set to distinguish 
the COVID-19 cases. 

![image](https://user-images.githubusercontent.com/58686831/197237579-52a2d79f-1795-4def-b2d7-7d929696fa6d.png)

**Result**

Confusion matrices and classification reports metrics were generated to 
evaluate model performance. In addition, other statistics were calculated for both models to 
identify the better models because both models showed very good performance. CNN2021 
model outperformed the TFVGG16 model with an average accuracy of 97.59 %±1.69 %. And 
also better prediction of Positive (COVID-19) cases based on the metrics of Precision, Recall 
and F1-score with average scoring of 95.63 ± 3.49 %, 97.05 ± 2.23 % and 96.33 ± 2.71 % 
respectively.  

![image](https://user-images.githubusercontent.com/58686831/197237655-013d7fa5-b370-4b8f-b343-de2bc24f469a.png)

![image](https://user-images.githubusercontent.com/58686831/197237705-46160023-ecca-4513-80d0-899c9e71d1d2.png)

![image](https://user-images.githubusercontent.com/58686831/197241071-9d1503c2-aad6-4202-8f1f-215cbb2bb1a4.png)

**Conclusion**

CNN2021 model was proven to be a better and effective model for this project experiment in a 
specific and limited data sample (2,500 – 13,000) on the specific binary classifying task 
(COVID-19 and Normal or Lung opacity) with average accuracy of 97.59 ±1.69%. CNN2021 
also delivered a good Precision, Recall and F1-score, better than TFVGG16 with an average 
value of 95.63±3.49%, 97.05±2.23% and 96.33±2.71% respectively. 

This project has explored the two deep neural network models with the knowledge and deep 
learning as well as the application of state-of-the-art transfer learning techniques. It was found 
that the simple CNN2021 model with lower hidden layers effectively detected the COVID-19 
chest X-rays images with lower error rates of false predictions compared to the model 
TFVGG16 which was developed with techniques of transfer learning. 

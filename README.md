# FER-System
Dataset used https://www.kaggle.com/datasets/deadskull7/fer2013

## Aim
One of the main aims of this study is to investigate the usage of deep learning for social robots
exclusively in the computer vision field. The problem tackled by the model is facial emotion recognition
as it is considered crucial for social interaction. The report will evaluate different proposed models of
deep learning. Then it will examine and discuss the effects of changing the hyperparameters of the
model. Also, the introduction of image and data prepressing is evaluated. All the experiments were
conducted using a single dataset created by (Verma, 2013) that contains around 30,000 facial images
categorised in 7 groups corresponding to common humane expressions (Angry, Disgust, Fear, Happy,
Sad, Surprise, Neutral). The data was then split into 80% training and 20% testing.

## Methodology
Although in many papers the use of a multiple data set is common. In this research a single dataset was
used which consists of 30,000 facial images because of the lack of time and processing limitation.
Of the first steps of this report is to select a model architecture that performs well in the dataset chosen.
The Four CNN models that were described in the previous section got analysed using K-fold cross
validation technique with K=5 using their recommended hyperparameters. Although the models had
impressive results in the papers, their performance was shocking ranging only from 40% to 50% except
for the model by (Mehendale, 2020) which averaged 65.57% correctness. I believe that the reason
behind these low performances is that the hyperparameters of the networks are not optimised for the
dataset. Also, it might be because the dataset contains a lot of noise. Nevertheless, because of the lack
of time, only the model by (Mehendale, 2020) was selected to be the base model of the FER system.
To improve the overall performance of the network, method inspired by different research papers where
used. Modifying the pre-processing approach used have been used to improve the performance of
model. Moreover, Previous studies deduced that the varying the hyperparameters significantly changes
the performance of the model. In this report the variation of several factors was evaluated such accuracy
* Vary in pre-processing approach: the number of classes
* Vary hyperparameters: learning rate, dropout value, number of layers and the number of neurons in each layer.
* Vary optimisation algorithm: Adam, Nadam and SGD optimisers were tested

# Chest-XRay-For-Classification

## Dataset - https://www.kaggle.com/haipham1202/chestx-ray14-v3

## Context: 
The given dataset, ChestX-ray14-v3, contains X-rays of three classes - Normal, Pneumonia, and Covid19. To improve the performance of the models, several preprocessing techniques were applied to the dataset. Gaussian, Median, and Mean filters were among the techniques used, and Gaussian filter proved to be more effective.

In addition to preprocessing techniques, various pre-trained models in Imagenet were used to classify the X-rays into their respective classes. These pre-trained models provided a great starting point for the task of image classification, and they were fine-tuned to improve their accuracy on the ChestX-ray14-v3 dataset.

By applying the above techniques, the accuracy of the model was improved up to 92%. This result indicates the effectiveness of the applied techniques in identifying different types of X-rays with high accuracy.

## Various Filters applied during Preprocessing:
![pre](https://user-images.githubusercontent.com/66003584/144365474-44edca21-ec9d-42da-9ce2-1cd7f9dcf607.PNG)

## Deep learning Models:
Den169, Inception V3, and VGG are all pre-trained convolutional neural network (CNN) models that can be used for image classification tasks. They have been trained on millions of images from the ImageNet dataset and have learned to identify different features and patterns in images.

When applied to X-ray images, these models can help classify them into different categories, such as normal, pneumonia, and COVID-19. The models can be fine-tuned on X-ray datasets to further improve their performance on this specific task.

Den169 is a lightweight version of the DenseNet model, which has shown promising results in image classification tasks with limited computational resources. Inception V3, on the other hand, uses a combination of convolutional and pooling layers to create a more complex model that can capture a wide range of image features. VGG is a widely used CNN architecture that uses multiple convolutional layers followed by max-pooling layers to create a hierarchical representation of an image.

By comparing the features learned by these models, we can get a better understanding of the features that are important for identifying different X-ray images. With appropriate preprocessing techniques and fine-tuning on the X-ray dataset, these models can achieve high accuracy in classifying X-ray images.

Ensembling DL Models:
Ensembling is a popular technique in machine learning, where multiple models are combined to make better predictions. In the context of classifying X-ray images, we can use an ensemble of the models DenseNet169, InceptionV3, and VGG to improve our classification accuracy.

There are different ways to combine the predictions of the models. One popular approach is to take a weighted average of their predicted probabilities. The weights can be determined using cross-validation or grid search techniques. Another approach is to use a majority voting scheme, where the final prediction is the class that receives the most votes from the models.

We can also experiment with different combinations of the models. For example, we can use only two of the models instead of all three, or we can use different weights for each model in the ensemble. By trying out different combinations and weighting schemes, we can potentially improve our classification accuracy and obtain more robust predictions.

Ensembling has been shown to be effective in many machine learning applications, and it can be particularly useful when dealing with complex datasets like medical images. However, it's important to note that ensembling also comes with some drawbacks, such as increased computational complexity and the need for more training data. Therefore, it's important to carefully evaluate the trade-offs and benefits of ensembling in each specific case.

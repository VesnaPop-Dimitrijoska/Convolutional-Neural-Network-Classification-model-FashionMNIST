# Project Title:
Convolutional Neural Network Classification model on Fashion MNIST Dataset
#
---
# Project Description:
Convolutional Neural Network Classification model on Fashion MNIST dataset which contains 70,000 grayscale images in 10 categories. 
#
---
# Table of Contents:

  1. Data analysis
  2. Data Preprocessing
  3. Data Augmentation
  4. Model Training
  5. Model Hyperparameter Optimization
  6. Model Prediction
  7. Model Evaluation
  8. Results Analysis
  9. Conclusion
#
---
# Dataset:
This guide uses the [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset which contains 70,000 grayscale images in 10 categories. 

Here, 60,000 images are used to train the network and 10,000 images to evaluate how accurately the network learned to classify images. 

The images show individual articles of clothing at low resolution (28 by 28 pixels), as seen here:

<table>
  <tr><td>
    <img src="https://tensorflow.org/images/fashion-mnist-sprite.png"
         alt="Fashion MNIST sprite"  width="600">
  </td></tr>
  <tr><td align="center">
    <b>Figure 1.</b> <a href="https://github.com/zalandoresearch/fashion-mnist">Fashion-MNIST samples</a> (by Zalando, MIT License).<br/>&nbsp;
  </td></tr>
</table>

---
# RESULTS
####
**Model Arhitecture**      
I tested multiple architectures and one of the best performances was achived with the model shown here.

Although the MaxPooling2D filter reduces the image by half, which in our case is quite small from the start, I used it in one of the models, because I think it was convenient for this type of images, that are containing a lot of contrast, because images are white on a black background. Performance was improved by nearly 0.5%. It was left out in my final model, and I think that it would improve the final model as well.

---
The best result was obtained using Data augmentation, although it was not recommended to use it in this kind of example, I tried it anyway to see if it would improve the result, and it did by nearly 2.5%. The training was extremly slow, so I didn't try this model combined with MaxPooling2D filter.     

![image](https://github.com/VesnaPop-Dimitrijoska/Convolutional-Neural-Network-Classification-model-FashionMNIST/assets/144008804/65784d23-8f85-4b31-afe1-6aab27cac086)

####
**Analyzing the predictions**  
    
From the histograms for each class, it is evident that the most similar classes are mixed the most: 'Shirt', 'Coat', 'Pullover', 'T-shirt/Top' and sometimes 'Dress'. The biggest confusion overal is between 'Shirt' and 'T-shirt/Top'.     
'Shirt' has lowest F1 score of all classes.
        
![image](https://github.com/VesnaPop-Dimitrijoska/Convolutional-Neural-Network-Classification-model-FashionMNIST/assets/144008804/c5a6a755-188e-4f08-a241-e96f899949d7) ![image](https://github.com/VesnaPop-Dimitrijoska/Convolutional-Neural-Network-Classification-model-FashionMNIST/assets/144008804/71d2f3c0-7be9-41b6-835b-bba9fa9f7c9d)

![image](https://github.com/VesnaPop-Dimitrijoska/Convolutional-Neural-Network-Classification-model-FashionMNIST/assets/144008804/7d2d940b-13b6-4d18-aa34-1537f1c6bb9c) ![image](https://github.com/VesnaPop-Dimitrijoska/Convolutional-Neural-Network-Classification-model-FashionMNIST/assets/144008804/f12ac040-55db-482a-81c3-1977c76e05e8)

---
#
# License
MIT License
#


# Image-Captioning

* A powerful deep powerful deep model that combines both image and text processing to generate textual description from an image based on the objects and actions in the image. Divided into two modules logically-one is an image based model which extracts the features from our image, the other is the language based model which translates the features and objects given by our image based model to a natural sentence.


![image](https://user-images.githubusercontent.com/59358031/158325030-727b60c7-e1a2-4570-b57f-4f42465026c0.png)

# - Dataset Description

* Flickr 8k dataset contains 8092 images and up to five captions for each image. Such annotations are essential for continued progress in automatic image description and grounded language understanding. They enable us to define a new benchmark for localization of textual entity mentions in an image. 

# - Some Visualization

### Input Image
<img src="https://user-images.githubusercontent.com/59358031/158332698-7da0e2d2-cdb5-4477-afc7-84570182515d.png" width=30% height=20%>

### Caption
 **A group of people standing in front of large building** 

### Input Image
<img src="https://user-images.githubusercontent.com/59358031/158332992-de6a8444-5447-46c5-8cde-2aea40cd7d4f.png" width=30% height=20%>

### Caption
**Race car is driving around track**

### Input Image
<img src="https://user-images.githubusercontent.com/59358031/158334720-a89a6c4c-6f91-4383-9bdf-621f9251f044.png" width=30% height=20%>

### Caption
**Brown dog is walking through snow**


# Explaining Encoder and Decoder
  ## Encoder: 
  ![alt text](https://github.com/raunak222/Image-Captioning/blob/master/Image/encoder.png)
  * For Encoder we use ResNet-50. ResNet-50 is a convolutional neural network that is trained on more than a million images from the ImageNet database. The network is 50 layers deep and can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. As a result, the network has learned rich feature representations for a wide range of images. The network has an image input size of 224-by-224.   

## Decode:
![alt text](https://github.com/raunak222/Image-Captioning/blob/master/Image/decoder.png)
* For Decoder we use LSTM. Long Short-Term Memory (LSTM) networks are a modified version of recurrent neural networks, which makes it easier to remember past data in memory. The vanishing gradient problem of RNN is resolved here. LSTM is well-suited to classify, process and predict time series given time lags of unknown duration. It trains the model by using back-propagation

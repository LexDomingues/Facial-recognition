# Facial Recognition of Messi and Cristiano Ronaldo using YOLO and CNN


This project was developed for the purposes of study, experimentation, and the practical application of concepts in supervised learning, convolutional neural networks, and computer vision.


**About the project**

This project aims to develop a computer vision system capable of detecting faces in images and recognizing whether the identified person is Lionel Messi or Cristiano Ronaldo.

The system combines two machine learning approaches: YOLO, which handles face detection, and a Convolutional Neural Network (CNN)—built using TensorFlow and Keras—which handles identity classification.

The project was developed for educational purposes, with the goal of applying concepts related to computer vision, supervised learning, and neural networks.


**Objectives**

Detect faces in images, including images containing multiple people.

Outline detected faces using bounding boxes.

Classify the faces as either Messi or Cristiano Ronaldo.

Integrate the detection and classification models into a single processing pipeline.

Evaluate the classifier's performance using metrics and charts.


**How it works**

The system is divided into three main stages:

1- Face detection with YOLO: Locates faces present in an image and returns their coordinates.

2- Face extraction: Uses the bounding box coordinates to crop each detected face.

3- Classification with CNN: Processes each cropped image and predicts whether it belongs to Messi or Cristiano Ronaldo.

Finally, the system displays the image with the bounding boxes and the names predicted by the classifier.


**CNN Training**

The CNN was built from scratch, without using pre-trained weights from another neural network.

Its architecture includes convolutional layers to extract visual features, max-pooling layers to reduce spatial dimensions, a dense layer for classification, and a dropout layer to help reduce overfitting.

The images are resized to 128 × 128 pixels. The output uses the sigmoid function to estimate the probability of one of the classes.


**Trained models**

The project uses two independent models:

YOLO face detector: locates faces within an image.

CNN classifier: identifies the faces as either Messi or Cristiano Ronaldo.

The trained models can be saved and loaded later, avoiding the need to repeat the training process.

**Limitations**

Performance may vary depending on lighting, resolution, face angle, the quality of the cropped images, and the degree of similarity between the input images and the training data.

An incorrect classification for a specific image does not necessarily mean that the entire system is failing. Therefore, evaluation should be based on a test set containing a diverse range of images.


**Results and evaluation**

<img width="536" height="455" alt="download" src="https://github.com/user-attachments/assets/df94d0d2-abb5-4102-8433-ca2a2ce1b0e0" />

Accuracy: 98.24%

Precision: 98.23%

Recall: 98.26%

F1-score: 98.24%

Error rate: 1.76%


**Use of AI**

Generative AI was used to support:

- Understanding concepts related to supervised learning, convolutional neural networks, and object detection.

- Assisting with the implementation and debugging of Python code.

- Investigating issues related to image pre-processing and the integration of models.

# **Classification: COVID-19 Detection using X-ray Images**

## **Overview**:
This project aims to detect COVID-19 using X-ray images. I used a Convolutional Neural Network to classify images as either indicative of a COVID-19 infection or not.

## **Project Structure**:

```
Classification_COVID19_using_XRay/
│
├── dataset/
│   └── data/
│       ├── train/
│       │   ├── COVID19/
│       │   └── NORMAL/
│       └── test/
│           ├── COVID19/
│           └── NORMAL/
│
├── images/
│   ├── covid1.jpg
│   ├── covid2.jpg
│   ├── normal1.jpg
│   └── normal2.jpg
│
└── README.md
```

This project is part of a fromation [course](https://www.coursera.org/projects/classification-of-covid19-using-chest-xray-images-in-keras) to learn about Convolutional Neural Network (CNN). The overall objective is to lear how to build and train a convolutional neural network using Keras with TensorFlow as a backend and how to apply augmentation techniques.
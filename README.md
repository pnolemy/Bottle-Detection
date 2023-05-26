# Bottle-Detection
# Project: Bottle and Can Detection for Events Security Gate

This project aims to develop an AI system that can detect bottles and cans using a camera for events security gates. The system will help enhance security measures by identifying prohibited items and triggering appropriate actions or alerts.

## Project Overview

The project consists of several tasks:

### Task 1: Data Acquisition

In this task, we collected a dataset of 195 pictures representing various scenarios encountered in events. The dataset was carefully curated to include diverse lighting conditions, angles, and backgrounds to ensure the AI model's robustness.

### Task 2: Data Preparation and Annotation

In Task 2, we prepared the collected dataset for training the AI model. Using the yolov5pytorch tool, we annotated each image by manually placing bounding boxes around the bottles and cans. This annotation step provided ground truth information necessary for training the model to recognize and detect these objects accurately.

### Task 3: Model Training and Deployment

Task 3 involved training the AI model using the annotated dataset. We utilized the powerful GPU support provided by Google Colab for efficient training. The yolov5pytorch framework was employed to train the model on the collected data, enabling it to learn the patterns and features associated with bottles and cans.
We trained with 110 epochs for 7.9 hours.

After training, we deployed the trained model to the Jetson Nano for edge computing. The Jetson Nano is an embedded system that allows for real-time inference, making it ideal for deployment at events security gates.

### Task 4: Model Inference

With the trained model deployed on the Jetson Nano, we can perform real-time inference on the video feed from the camera at the events security gate. The model analyzes each frame from the video stream, detecting the presence and location of bottles and cans. This enables immediate actions or alerts to be triggered for security personnel, ensuring swift response to any prohibited items.

## Model Performance and Logging

During the model training process, we monitor the performance of the AI model and log relevant metrics to assess its progress. Key considerations include:

- **Model Performance Evaluation**: We evaluate metrics such as loss, precision, recall, and average precision (AP) to measure the model's accuracy and effectiveness in detecting bottles and cans.

- **Logging and Visualization**: We utilize tools like TensorBoard to log and visualize training metrics. TensorBoard provides interactive charts and graphs to monitor the model's learning behavior over time. Metrics such as loss and AP are logged, enabling detailed analysis and informed decisions for model optimization.

Please refer to the project's documentation and code for more detailed instructions on data preparation, model training, and deployment.

## Contributors

1. Mr.Piriyapol Prasankliew ID:64011563
2. Ms.Sirapatsorn Saksopa ID:64011613
3. Mr.Kochbhabob Vongbandit ID:64011437
4. Mr.Jirayus Phonphruksa ID:64110096

## Acknowledgments

This project is part of the Robot Lab3 Robotics and AI Engineering program at KMITL School of Engineering. We would like to express our gratitude to the faculty and staff for their guidance and support throughout the project.

Project Description:

The Human-and-Animal-detection-in-flooded-areas-using-YOLO is a computer vision project that aims to automatically identify humans and animals in flooded areas using deep learning techniques, known as Humans-and-Animals-detection-in-flooded-areas-using-YOLO. The project uses the YOLO (You Only Look Once) object detection architecture to process drone/satellite or ground level images. The goal of the project is to support the rescue operation/disaster response by locating situations where there is a living being that may require immediate assistance.

Key Features:

Deep Learning Model: Uses convolutional neural networks (CNN) utilizing the YOLO framework to perform real-time object detection in areas of substantial clutter (natural and built) that are prone to floods. 

Data Interaction: Loads and pre-processes image datasets, separating the images into training and test datasets. Models were trained and validated on a curated dataset, achieving a high degree of training and validation accuracy during initial trials.

Layered Model Architecture: The CNN implemented has several layers comprising of  Conv2D, MaxPooling2D, Flatten, and Dense Layers, for a total of over 11 million trainings parameters and robustness for precise detection functions.

Training Pipeline: The project is configured for repeatable training with Keras/TensorFlow in Python, typically in environments such as Google Colab. An early stopping criteria was used to avoid overfitting, and this restored the best weights automatically.  

Real-world Application: The COG project was built to support human emotional sensing and potential live-saving scenarios, while providing an easily translatable visual representation of ability to detect persons, and integrate with mapping and geospatial information system (GIS) tools for real-time disaster-ready environment.

Usage:

Environment: Python with the TensorFlow and Keras libraries (using Google Colab is recommended because of hardware acceleration and seamless integration with Google Drive).

Data Organization: The images are organized in folders in Google Drive to help facilitate ease of access in the example code. You'll need to update any paths in the notebook so they match your own folder structure. 

Running the Model: You can run each cell of the notebook in order from top to bottom. The code will mount your drive, load the data, build your model, run your training process, and print performance metrics.

Dataset:

Source: User-provided images stored in a Google Drive with two directories of images: train and test, which each have images of animals and humans annotated in flood situations.

Shape: In total, the Training set had 477 images and Test set had 78 images. Overall, all images were re-sized to be 224px x 224px large for processing purposes.

Results:

This model achieved nearly perfect performance on the provided images. This indicates a strong ability to detected people and animals in test data that had never been seen before but I would recommend further validation on real-life, much more diverse datasets.

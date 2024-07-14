# Vehicle Movement Analysis and Insight Generation in a College Campus using Edge AI.

### Introduction

Talking about the problem statement, in many buildings such as colleges,hospitals,apartments keeping track of the vehicles is a challenge.Whether the vehicles is allowed to enter to the building, is there any parking slots left for vehicle and many more challenges so The aim of our project is to develop a system which can generate the insights of vehicles in college campus.This system can capture the real time images via camera or webcam and can detect the vehicle license plate numbers and generate the insights for that particular vehicle.

### Objective

The objective of this project is to detect the vehicles license plates from images to text in real time.Check whether the vehicle is allowed into the building or not and finally to know the parking occupancy in the building. 

### Dataset

The dataset used can be downloaded from Kaggle.[Dataset](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection).
In TensorFlow we have divided the dataset into two parts one is test and the other is train. 

### Methodology

1. **Image Acquisition**
   - Capture real-time images using a webcam feed or use pre-existing images.

2. **Object Detection using TensorFlow**
   - Utilize TensorFlow Object Detection to identify and isolate the region of interest (ROI), which in this case is the number plate.
   - The detection model will be trained on a [Kaggle dataset](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection) to accurately identify number plates in various conditions.

3. **Text Extraction using EasyOCR**
   - Employ EasyOCR to extract the alphanumeric characters from the detected number plate.
   - Implement a size filtering algorithm to focus on the largest detection region, ensuring the most accurate text extraction.
  
### Steps

1. **Setup**
   - Initial setup and configuration for the project, including installing necessary libraries and dependencies.

2. **Cloning Baseline Code**
   - Clone the baseline code repository to use as a starting point for the project.

3. **Creating a Virtual Environment**
   - Set up a virtual environment to manage project dependencies and ensure a consistent development environment.

4. **Installing Dependencies**
   - Install all required libraries and dependencies, including TensorFlow and EasyOCR.

5. **Installing TensorFlow Object Detection**
   - Install and configure TensorFlow Object Detection API.
   - Train the model on a Kaggle dataset to detect number plates.

6. **Implementing the Detection and OCR Pipeline**
   - Capture images from the webcam or load pre-existing images.
   - Apply the TensorFlow Object Detection model to locate the number plate in the image.
   - Use EasyOCR to extract the text from the detected number plate region.
   - Apply size filtering to improve the accuracy of the OCR process.
7. **Checking the Vehicles**
   - Save a few images taken through the webcam.let them be apporved vehicles.
   - convert the number plate into string and store it.
   - Using binarysearch check whether the vehicle is allowed or not.
      



### Conclusion

With this project we can develop a tool which can accurately detect the number plates , generate the text out of image , perform the vehicle matching,parking lot occupancy and insight generation.



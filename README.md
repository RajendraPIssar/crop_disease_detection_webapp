# Crop Disease Detection Web Application

This web application allows users to detect crop diseases using images captured via a webcam or uploaded manually. It utilizes a pre-trained deep learning model to classify the crop's health as either **Healthy**, **Stem Rust**, or **Leaf Rust**. The application also includes a video feed that enables real-time image capture for disease prediction.

## Features

- **Real-Time Image Capture**: Capture images using a webcam and predict crop diseases.
- **Image Upload**: Upload crop images and get disease predictions.
- **Disease Classification**: Classifies crops into three categories: Healthy, Stem Rust, and Leaf Rust.
- **Image Display**: Displays the uploaded or captured image with the predicted label.

## Tech Stack

- **Backend**: Flask
- **Frontend**: HTML, CSS (Bootstrap)
- **Machine Learning**: TensorFlow, Keras
- **Image Processing**: OpenCV, Pillow
- **Other Libraries**: NumPy, Random

## Prerequisites

Before you can run the project, make sure you have the following installed:

- Python 3.x
- Flask
- TensorFlow/Keras
- OpenCV
- Pillow (PIL)
- NumPy
  
**Model Details**
The application uses a pre-trained convolutional neural network (CNN) model saved as model_0.h5. The model expects input images resized to (256x256) pixels, and the pixel values are normalized before feeding them to the model for prediction.

You can either train your own model using TensorFlow/Keras or use a publicly available model trained on similar data. For best results, ensure that the model is trained on crop disease datasets.
## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/crop-disease-detection.git
   cd crop-disease-detection
2. **Install dependencies**:
Install the required Python libraries by running the following command:


```bash
  pip install -r requirements.txt


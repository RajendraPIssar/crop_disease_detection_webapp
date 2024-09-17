# crop_disease_detection_webapp

This web application is designed to detect crop diseases using images captured via webcam or uploaded by users. The project leverages a pre-trained deep learning model to classify crop health as "Healthy," "Stem Rust," or "Leaf Rust" based on the input image. The app also includes a video feed that allows users to capture images in real time using a webcam.

Features
Real-time image capture using a webcam.
Upload images for disease prediction.
Classification of crop disease: Healthy, Stem Rust, or Leaf Rust.
Displays the uploaded or captured image along with the disease prediction.
Tech Stack
Backend: Flask
Frontend: HTML, CSS (with Bootstrap templates)
Machine Learning Framework: TensorFlow, Keras
OpenCV: For video capture and image processing
Additional Libraries: PIL, NumPy
Prerequisites
To run this project locally, you need to have the following installed:

Python 3.x
Flask
TensorFlow/Keras
OpenCV
PIL (Pillow)
NumPy
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/crop-disease-detection.git
cd crop-disease-detection
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Ensure you have the following directories created within the static folder:

arduino
Copy code
static/shots
Download or load the trained model model_0.h5 into the project folder.

Run the application:

bash
Copy code
python app.py
Open your browser and go to http://127.0.0.1:5000/ to access the web application.

Directory Structure
bash
Copy code
.
├── app.py                    # Main Flask application
├── templates/                # HTML files
│   ├── index.html            # Homepage
│   ├── input.html            # Image input form
│   └── display.html          # Displays result
├── static/
│   └── shots/                # Stores captured/uploaded images
├── model_0.h5                # Pre-trained machine learning model (download separately)
├── requirements.txt          # Project dependencies
└── README.md                 # Project documentation
Usage
Navigate to the homepage.
You can either:
Capture an Image: Start the webcam and click "Capture Image."
Upload an Image: Use the upload feature to select a crop image from your local machine.
The application will display the captured/uploaded image along with the predicted crop health status (Healthy, Stem Rust, or Leaf Rust).
Allowed File Types
PNG
JPG
JPEG
GIF
Webcam Integration
The webcam feature is enabled using OpenCV. When you click "Capture Image," it saves the frame from the webcam feed to the static/shots folder, where it is processed for disease detection.

Model Training
The application uses a pre-trained deep learning model saved as model_0.h5 that you need to add to your project. The model expects input images resized to (256x256) pixels and normalizes the pixel values before prediction.

License
This project is open-source and available under the MIT License.

Feel free to modify any sections as per your specific project details. If you need to create a requirements.txt file for this project, you can generate it using:

bash
Copy code
pip freeze > requirements.txt

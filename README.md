# OpenCV Face and Eye Detection in Flask Web Framework

This project demonstrates face and eye detection in real-time using OpenCV integrated within a Flask web application. By leveraging the power of OpenCV's pre-trained models and Flask's lightweight web framework, this application captures webcam video and applies face and eye detection.

## Features

- **Real-time face and eye detection**: Detects faces and eyes from a live webcam feed and displays the results in a browser.
- **Flask web interface**: Stream the webcam feed and the detected features through a simple web interface.
- **Pre-trained models**: Utilizes OpenCV's Haar Cascade Classifiers for fast and accurate detection.
- **Lightweight and easy-to-extend**: A minimal project structure that is easy to understand, modify, and extend.

## Prerequisites

Before running this project, ensure you have the following installed:

- Python 3.x
- Flask (`pip install flask`)
- OpenCV (`pip install opencv-python`)

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/SubhankarChand/OpenCV-Face-And-Eye-Detection-In-Flask-Web-Framework.git
    cd OpenCV-Face-And-Eye-Detection-In-Flask-Web-Framework
    ```

2. **Install required dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the application**:

    ```bash
    python app.py
    ```

4. **Access the detection stream**:

   Open your web browser and navigate to:

    ```
    http://127.0.0.1:5000
    ```


- **`templates/index.html`**: The HTML file that renders the video stream with the detected face and eye bounding boxes.
- **`app.py`**: The main Python script that integrates OpenCV and Flask for video streaming and detection.
- **`haarcascades/`**: This folder contains the Haar Cascade XML files for face and eye detection.
- **`requirements.txt`**: Lists the required Python libraries to run the project.
- **`README.md`**: The project documentation (this file).

## Code Explanation

1. **Face and Eye Detection**:
   - The project uses OpenCV's `haarcascade_frontalface_default.xml` and `haarcascade_eye.xml` files to detect faces and eyes in real time.
   
2. **Webcam Capture**:
   - The `cv2.VideoCapture(0)` command is used to capture the video feed from the system's webcam.
   
3. **Frame Processing**:
   - Each frame is processed to detect faces and eyes, and bounding boxes are drawn around the detected regions before being streamed.

4. **Flask Integration**:
   - The application streams the processed video feed using Flask’s `Response` object with the MIME type set to `multipart/x-mixed-replace`.

## Example Output

Once the app is running, you should see a live video stream in your browser with real-time face and eye detection.

## Contributing

Contributions are welcome! Feel free to fork this repository, submit pull requests, or open issues for suggestions and improvements.



### Author

Developed by [Subhankar Chand](https://github.com/SubhankarChand).



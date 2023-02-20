# Image-to-Sketch-Conversion
Capture an image from video and convert it into sketch using OpenCV python.

    
    This is a Python project that uses OpenCV to perform real-time sketch conversion on a live video stream. The program takes input from a camera or video file and produces a live sketch video stream in real-time.
    
### Installation
To run this program, you need to install OpenCV and NumPy. You can do this using the following commands:

    pip install opencv-python
    pip install numpy

### Usage
    
    Provide permission to your ide to the access webcam 
    
To run the program, navigate to the directory containing the live_sketch.py file and run the following command:

    python live_video-to-sketch.py    
    The program will automatically detect your default camera and start producing a live sketch video stream. 
    To exit the program, press the 'q' key on your keyboard.
    If you want to use a video file instead of a live camera feed, you can modify the code to use a video file instead.

### How it works

The program works by applying a series of image processing operations to each frame of the input video stream. Specifically, the program performs the   following steps:

    1. Capture a frame from the input video stream.
    2. Convert the color image to grayscale.
    3. Apply a Gaussian blur to the grayscale image to smooth out any noise.
    4. Detect the edges in the blurred image using the Canny edge detection algorithm.
    5. Invert the colors of the edge image.
    6. Combine the inverted edge image with the original grayscale image to create a sketch-like effect.

These steps are performed on each frame of the input video stream to produce a real-time sketch video stream.

### Output:

<img width="1279" alt="generated_Sketch" src="https://user-images.githubusercontent.com/90651908/219996453-709175a1-2ff6-48a7-8dd8-3ec98d4531e0.png">


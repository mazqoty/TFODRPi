# TFODRPi

Steps
1. Generate TFLite Files: by executing '2.Colab_Training_and_Detection.ipynb' file in [TFOD Repository](https://github.com/mazqoty/AI-in-Quality-Control) OR DOWNLOAD THE GIVEN MODEL
2. Clone the current repository onto your Rasberry Pi or copy it from a machine using RDP.
3. Install the required dependencies onto your Rasberry Pi.

`pip3 install opencv-python`<br>
`sudo apt-get install libcblas-dev`<br>
`sudo apt-get install libhdf5-dev`<br>
`sudo apt-get install libhdf5-serial-dev`<br>
`sudo apt-get install libatlas-base-dev`<br>
`sudo apt-get install libjasper-dev`<br>
`sudo apt-get install libqtgui4`<br>
`sudo apt-get install libqt4-testv`<br>
`echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list`<br>
`curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -`<br>
`sudo apt-get update`<br>
`sudo apt-get install python3-tflite-runtime`<br>

4. Copy your detect.tflite model into the same repository and update the labels.txt file to represent your labels.
5. Run real time detections using the detect.py script
- `python3 detect.py`

# Resources

Based on https://github.com/tensorflow/examples/blob/master/lite/examples/object_detection/raspberry_pi/README.md

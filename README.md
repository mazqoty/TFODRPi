# TFODRPi

Steps
1. Generate TFLite Files: by executing '2.Colab_Training_and_Detection.ipynb' file in [TFOD Repository](https://github.com/mazqoty/AI-in-Quality-Control)
2. Clone the current repository onto your Rasberry Pi or copy it from a machine using RDP.
3. Install the required dependencies onto your Rasberry Pi.

`pip3 install opencv-python`
`sudo apt-get install libcblas-dev`
`sudo apt-get install libhdf5-dev`
`sudo apt-get install libhdf5-serial-dev`
`sudo apt-get install libatlas-base-dev`
`sudo apt-get install libjasper-dev`
`sudo apt-get install libqtgui4`
`sudo apt-get install libqt4-testv`
`echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list`
`curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -`
`sudo apt-get update`
`sudo apt-get install python3-tflite-runtime`

4. Copy your detect.tflite model into the same repository and update the labels.txt file to represent your labels.
5. Run real time detections using the detect.py script
`python3 detect.py`

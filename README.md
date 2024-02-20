# Real-Time Object Detection with OpenCV, MobileNet v3 Large, and COCO

This project demonstrates real-time object detection using:

* OpenCV's DNN module for computer vision tasks.
* The pre-trained MobileNet v3 Large model, known for its efficient and accurate object recognition.
* The COCO dataset, providing a diverse range of object class names for broader detection capabilities.

### Features

* Leverages MobileNet v3 Large for fast and accurate object detection.
* Utilizes the COCO dataset's diverse object classes, suitable for various detection tasks.
* Visualizes detected objects with bounding boxes and corresponding class labels for clear understanding.

### Requirements

* OpenCV with DNN module (installation guide: [https://opencv.org/](https://opencv.org/))
* Pre-trained MobileNet v3 Large model weights (`frozen_inference_graph.pb`) and configuration file (`ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt`)
* COCO dataset class names file (`coco.names`)

### Usage

1. **Download:** Place the required files (mentioned above) in the same directory as your Python script.
2. **Run:** Execute the script from the command line:

   ```bash
   python object_identification_photo.py
3. **Input:** The script expects a test image named lena.png to be present in the same directory.

### Code Walkthrough
The provided Python script performs the following steps:

- Loads the test image (lena.png).
- Reads the COCO dataset class names for reference.
- Loads the pre-trained MobileNet v3 Large model configuration and weights.
- Configures the model's input parameters for optimal performance.
- Detects objects in the image with a minimum confidence threshold (adjustable).
- Draws bounding boxes around detected objects and displays their corresponding class names.
- Displays the final image with annotations.
Note: The code snippet provided is for illustrative purposes. Refer to the actual script for details.

### Customization
- Modify the test image name (lena.png) to use a different image for detection.
- Adjust the confThreshold value in the script to control the minimum confidence level for object detection.
- Explore and experiment with different pre-trained models and datasets beyond COCO to suit your specific needs and detection tasks.

### Additional Notes
- This script showcases a basic object detection example. You can extend it to handle video streams, track detected objects, customize bounding box styles, and display additional information.
- Consider experimenting with different models, object classes, and input sources to explore the wide range of possibilities for object detection.
- Ensure you have correctly installed and structured the required dependencies and files before running the script.

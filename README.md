PMN-Subaqueous-Detection-GUI

PMN-Subaqueous-Detection-GUI is a Python-based graphical user interface (GUI) application for underwater multi-object detection, designed to analyze images, videos, and real-time camera feeds for marine entities such as fish, coral, algae, reefs, and polymetallic nodules (PMN). It integrates advanced computer vision models, including YOLO, Haar Cascade, and Faster R-CNN, with a Tkinter-based interface. Usage, modification, or distribution of this software requires explicit written permission from the author.
Features

Multi-Object Detection: Detects fish, coral, algae, reefs, and PMN in underwater images and videos.
Real-Time Processing: Supports single and multiple camera inputs, including IP cameras.
Model Compatibility: Supports YOLO (.pt), Haar Cascade (.xml), and Faster R-CNN (.pth) models.
Configurable Parameters: Adjust minimum neighbors, scaling factor, and focal length for precise detection.
Result Outputs: Displays counts of detected flora, fauna, nodules, algae, approximate frame area, and camera-seabed distance.
Camera Management: Configure up to four IP cameras for real-time analysis.

Requirements
To run PMN-Subaqueous-Detection-GUI, ensure you have the following installed:

Python 3.8 or higher
Tcl/Tk 8.6 (typically bundled with Python)
Required Python packages (listed in requirements.txt):Pillow>=9.0.0
opencv-python>=4.5.5
torch>=2.0.0
torchvision>=0.15.0
ultralytics>=8.0.0
numpy>=1.21.0



Install dependencies using:
pip install -r requirements.txt

Installation

Request Access: Contact Wilfred Auxilian at wilfred.auxilian@example.com to obtain permission to use the software. You may also reach out via LinkedIn at [www.linkedin.com/in/wilfred-auxilian-george-55851127b].
Clone the repository (if granted access):git clone https://github.com/wilfredauxilian/PMN-Subaqueous-Detection-GUI.git
cd PMN-Subaqueous-Detection-GUI


Install the required dependencies:pip install -r requirements.txt


Obtain pre-trained model files (.pt, .xml, or .pth) for the datasets you wish to analyze (fish, coral, algae, reef, PMN).

Usage
Note: You must obtain written permission from Wilfred Auxilian before using or modifying this software.

Run the application:python main.py


Load Input:
Click "Browse Image" or "Browse Video" to select an image (.png, .jpg, .jpeg, .bmp) or video (.mp4, .avi, .mov).


Select Datasets:
Check boxes for FISH, CORAL, ALGAE, REEF, or PMN and select corresponding model files (.pt, .xml, .pth).


Configure Parameters:
Min Neighbour: Set for Haar Cascade detection sensitivity (0–300).
Scaling Factor: Adjust for Haar Cascade scaling (1.0–10.0).
Focal Length: Enter the camera’s focal length (in mm) for distance calculations.


Configure IP Cameras:
Enable the "IP CAMERAS" checkbox and enter valid IP addresses in the camera fields.


Process Input:
Click "Apply changes" to run detection and display annotated results.


View Results:
Annotated images/videos are shown in the main display window.
Detection counts (flora, fauna, nodules, algae), frame area, and camera-seabed distance are displayed in the "RESULT" section.



Example

Obtain permission from Wilfred Auxilian.
Load an underwater image (sample.jpg).
Select a YOLO model for fish detection (fish.pt) and a Haar Cascade for coral (coral.xml).
Set Min Neighbour=5, Scaling Factor=1.2, and Focal Length=35.
Click "Apply changes" to view the annotated image and detection metrics.

Project Structure
PMN-Subaqueous-Detection-GUI/
├── main.py              # Main application script
├── support.py           # Support functions (assumed)
├── requirements.txt     # Dependencies
├── LICENSE.md           # Proprietary License
├── README.md            # This file
└── models/              # Directory for model files (not included)

Notes

Model Files: Place pre-trained model files in a models/ directory or specify their paths when prompted. Models are not included in this repository due to size constraints and licensing restrictions. Contact Wilfred Auxilian at wilfred.auxilian@example.com for access to models.
IP Camera Support: Ensure IP addresses are valid and cameras are accessible on the network.
Performance: For optimal performance, use a GPU with CUDA support for YOLO and Faster R-CNN models.
Dependency Licenses: Users must comply with the licenses of dependencies (e.g., YOLO’s AGPL-3.0, OpenCV’s Apache 2.0). This software’s proprietary license applies only to the code in this repository.
Support File: The application assumes a support.py file (based on the import of SAM5_support). Ensure it is included or adjust the code if not required.

License
This project is licensed under a proprietary license. No usage, modification, or distribution is permitted without prior written consent from Wilfred Auxilian. See the LICENSE.md file for details. Contact Wilfred Auxilian at wilfred.auxilian@example.com to request permission.
Contact
For permission requests or questions, contact Wilfred Auxilian at wilfred.auxilian@example.com or via LinkedIn at [www.linkedin.com/in/wilfred-auxilian-george-55851127b].

Generated by Wilfred Auxilian

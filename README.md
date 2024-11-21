# Poppy Detection AI using YOLOv5

This project is an AI-based detection system for poppies (Papaver rhoeas) using YOLOv5, a state-of-the-art object detection framework. The model is trained to recognize poppies in images and videos with high accuracy.

## Features
- **Real-time Detection**: Detect poppies in real-time from video streams or images.
- **Custom Dataset**: Trained on a custom dataset specifically curated for poppy recognition.
- **Scalable**: Easily adaptable for detecting other types of flowers or objects with minimal changes.

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<repository-name>.git
   cd <repository-name>
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
3.	Install YOLOv5:
  Follow the installation instructions from the official YOLOv5 repository.
Dataset

The model was trained on a custom dataset of poppy images:
	•	Number of Images: X images
	•	Annotations: Labeled in YOLO format using tools like LabelImg or Roboflow.
	•	Data Augmentation: Applied transformations including rotation, scaling, and flipping to enhance model robustness.
 
 Directory Structure
 <repository-name>/
├── data/
│   ├── images/
│   ├── labels/
├── models/
├── runs/
├── detect.py
├── train.py
└── README.md

Usage

Detection

To run the detection model on an image or video:
   ```bash
python detect.py --weights best.pt --source <path-to-image-or-video>
```
Training
   ```bash
python train.py --img 640 --batch 16 --epochs 50 --data data.yaml --weights yolov5s.pt
```
To train the model on your custom dataset:

Example
Results

	•	mAP@0.5: XX%
	•	Inference Time: XX ms per image
	•	Training Time: XX hours on GPU

Future Plans

	•	Expand dataset for improved generalization.
	•	Add multi-flower detection capability.
	•	Integrate with Drones and OpenCV: Plan to use this AI model in a surveillance drone system for security purposes. The drone will scan large areas using OpenCV for image processing and detect illegal poppy plantations in real-time.

Contributing

Contributions are welcome! Feel free to fork this repository and submit a pull request with your changes.

License

This project is licensed under the MIT License. See the LICENSE file for more details.

Acknowledgments

	•	Ultralytics YOLOv5 for the detection framework.
	•	Open-source contributors for making tools like LabelImg and Roboflow available.

Contact

For any questions or suggestions, please feel free to contact me at [gjw3067@gmail.com].

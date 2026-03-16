# Animal Detection with YOLO

## Project Details

This project is focused on detecting various animal species using the YOLO (You Only Look Once) framework.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Kif30/animal-detection-with-yolo.git
   cd animal-detection-with-yolo
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. Prepare your dataset in the specified format.
2. Run the training script:
   ```bash
   python train.py --data data.yaml --cfg yolov3.cfg --weights yolov3.weights
   ```
3. To perform inference on images:
   ```bash
   python detect.py --weights yolov3_weights.pt --source path/to/image.jpg
   ```

### Features
- Real-time animal detection.
- Supports multiple species detection.
- Easy to adapt for different datasets.

### Tech Stack
- Python
- OpenCV
- YOLO (Darknet)
- TensorFlow/Keras (for training)

### How It Works
The YOLO framework breaks the input image into a grid and assigns bounding boxes and class probabilities to those boxes. The model's output consists of bounding boxes, class id, and confidence scores for detected objects.

### Model Details
- The model utilized is YOLOv3, which is known for its speed and accuracy in object detection tasks.

### Dependencies
- TensorFlow
- NumPy
- OpenCV
- Pillow
- Matplotlib

### Custom Training Tips
- Ensure your dataset is well-annotated and balanced.
- Experiment with different learning rates.
- Use data augmentation to improve model robustness.


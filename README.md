🩸 Hemoglobin Level Detection using Deep Learning and Instance Segmentation

This project presents an AI-powered pipeline for Hemoglobin (HB) level detection using eye images. The system combines instance segmentation and deep learning classification to identify anemia-related patterns from conjunctiva images.

The project uses:
Detectron2 Mask R-CNN for eye/conjunctiva segmentation
MobileNetV2 for HB level classification
TensorFlow & PyTorch for model development

🚀 Features
Eye region segmentation using Mask R-CNN
Automatic extraction of segmented conjunctiva area
Deep learning-based anemia classification
Transfer learning with MobileNetV2
COCO-format dataset training support
End-to-end inference pipeline
Google Colab compatible

🧠 Pipeline Overview
1️⃣ Eye Segmentation
Detects conjunctiva region from eye images
Uses Detectron2 Instance Segmentation
Generates segmented mask images
2️⃣ Feature Extraction
Extracts segmented eye region
Resizes and preprocesses images
3️⃣ Hemoglobin Classification
Uses MobileNetV2 Transfer Learning
Predicts:
Low HB (Anemia)
Normal HB

🛠️ Technologies Used
Python
TensorFlow / Keras
PyTorch
Detectron2
OpenCV
Roboflow
MobileNetV2
NumPy / Pandas / Matplotlib

📂 Dataset
The segmentation dataset is trained using:
COCO segmentation annotations
Roboflow dataset management

Dataset includes:
Eye/conjunctiva images
Segmentation masks
HB classification labels

⚙️ Installation
Install dependencies:
pip install tensorflow torch torchvision
pip install opencv-python matplotlib pandas numpy
pip install roboflow
pip install 'git+https://github.com/facebookresearch/detectron2.git'

📊 Model Architecture
🔹 Segmentation Model
Mask R-CNN R101-FPN
Detectron2 framework
Instance segmentation for conjunctiva extraction
🔹 Classification Model
MobileNetV2
Transfer learning from ImageNet
Binary classification

🧪 Training
Segmentation Training
trainer = DefaultTrainer(cfg)
trainer.resume_or_load(resume=False)
trainer.train()
Classification Training
history = model.fit(
    x=x,
    y=y,
    batch_size=32,
    epochs=20,
    validation_split=0.2
)

🔍 Inference Pipeline
The system:
Segments eye region
Extracts conjunctiva area
Runs HB classification
Predicts anemia status

Example Output:
HB level is low
or
HB level is normal

📈 Applications
AI-assisted anemia screening
Non-invasive HB estimation
Healthcare computer vision systems
Medical image analysis
Smart diagnostic systems

📜 License
This repository is intended for research and educational purposes only.

🤝 Contributions
Contributions and improvements are welcome.

⭐ Project Highlights
✔ Instance Segmentation
✔ Medical Image Processing
✔ Transfer Learning
✔ End-to-End Deep Learning Pipeline
✔ Detectron2 + TensorFlow Integration
✔ Healthcare AI Application

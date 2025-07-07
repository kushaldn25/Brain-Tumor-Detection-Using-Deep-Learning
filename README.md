# Brain-Tumor-Detection-Using-Deep-Learning

# Objective:

The objectives of the process of detection of Brain Tumor using MR image analysis are broadly divided. Study of pre-processing of MR images. Image acquisition Adaptive filtering Study of Image Analysis of MR images Segmentation Feature Extraction Enhancement Development of neural network algorithm for Classification and Detection of Brain Tumor. Magnetic resonance imaging method is widely used for detecting the model of the tumor developed in human brains. Manual detection of tumors is very difficult. Manual process which is carried out is also susceptible to failure in critical preoperative situations and causes overall increased operating time and healthcare costs .When faced with a patient with brain tumor surgeons have to change the modular components and the liner, that is why it is crucial to know the tumor model before the surgery starts to avoid any kind of operative failures.

# Introduction:

Brain tumors are abnormal or uncontrolled growths in the brain cells, which can be benign or malignant, with varying types like gliomas, meningiomas, and metastatic tumors. They can be primary (originating in the brain) or secondary (spreading from other organs). A tumor alters normal brain activities, which can result in symptoms like headaches, seizures, memory loss, difficulty speaking, cognitive issues. Early detection of brain tumors improves survival rates and treatment outcomes, preventing severe neurological damage and enabling timely interventions like surgery, radiation, or chemotherapy.

Magnetic Resonance Imaging (MRI) is a non-invasive imaging technique that uses strong magnetic fields and radio waves to create clear and precise images of soft tissues, making it highly effective in identifying tumors, their location, and their effect on surrounding brain areas.
Furthermore, advanced MRI techniques, such as contrast-enhanced MRI and functional MRI (fMRI), provide deeper insights into tumor characteristics, helping doctors plan the most appropriate treatment strategies. Its accuracy, non-invasive nature, and ability to detect even small abnormalities make MRI the gold standard for brain tumor diagnosis.

Deep learning, Deep Learning, a subset of Machine Learning, has transformed medical imaging by making MRI analysis faster, more accurate, and automated. In traditional machine learning, radiologists and engineers must define specific features such as tumor shape, texture, or intensity, which can be time-consuming and prone to human bias. However, this approach often fails when tumors vary in size, shape, or contrast due to differences in imaging conditions.
Unlike traditional machine learning, which requires manual feature extraction, deep learning models learn patterns directly from raw images, making them particularly effective for complex visual data like brain MRIs.

# Motivation:

However, despite advancements in medical imaging, there are still research gaps that challenge efficient and accurate tumor detection, motivating the need for further study:
Limitations of Traditional Machine Learning
Existing Models Lack Real-Time Efficiency
High Computational Cost and Lack of Lightweight Models
Our project aims to overcome these issues by combining YOLOv10 for real-time detection.

# Methodology:

## Data Preparation
Image Conversion: 3D MRI scans were split into 2D images
Resizing: All images resized to 256×256 pixels 
Annotations:(i)YOLO: Bounding boxes in .txt files.
Cleaning and Normalization: Removed images with no tumors or poor quality and Normalized [0,1] pixel intensities.

## Exploratory Data Analysis (EDA)
Visually inspected central slices to ensure image quality, tumor presence, consistent intensity, and accurate labels.

## System Architecture
YOLOv10 – Detection
Detects and draws bounding boxes around tumors quickly.and Ideal for real-time use 

## Model Evaluation
YOLOv10 was assessed using mAP for detection accuracy and FPS for speed. 
ResUNet was evaluated with Accuracy, IoU, and Dice Score to measure pixel-level segmentation performance..

# Conclusion:

This project addresses a major challenge in brain tumor diagnosis: achieving a balance between speed and accuracy. To tackle this, we implemented a model framework using YOLOv10 for real-time tumor detection. The models were trained and evaluated on the BraTS2020 dataset, with extensive preprocessing and fine-tuning to ensure high performance. Our approach enables rapid tumor localization through YOLO, making it highly suitable for intraoperative use. To enhance usability, we developed a Gradio-based graphical user interface (GUI), allowing medical professionals to interact with the system without any programming knowledge. Overall, this work lays the groundwork for an intelligent, real-time AI assistant that can reduce diagnostic errors, enhance decision making, and significantly improve patient outcomes in neuro-oncology.


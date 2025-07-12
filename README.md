# 🐾 Animal Detection and Alert System using Raspberry Pi 4

This project provides a smart and automated solution for detecting wildlife in remote areas using Raspberry Pi 4, sensors, and a machine learning model. It aims to prevent human-wildlife conflict by identifying animals, storing their images in the cloud, and sending SMS alerts to local authorities or residents in real time.

##  Project Overview

Wildlife intrusion into human habitats is increasing due to urbanization and habitat loss. Our system detects, identifies, and notifies the presence of wild animals to reduce potential harm to both humans and animals.

-  **Captures animal images using a USB webcam**
-  **Identifies animals using a CNN model (VGG19-based)**
-  **Uploads images to Google Drive**
-  **Sends SMS alerts via SMSChef API**

---

##  Hardware Requirements

- Raspberry Pi 4 Model B
- USB Webcam
- Ultrasonic Sensor
- MicroSD Card (with Raspberry Pi OS)
- Power Supply (5V)

---

##  Software Requirements

- **OS**: Raspberry Pi OS
- **Language**: Python (Thonny IDE)
- **Libraries**:  
  - `OpenCV`  
  - `TensorFlow`, `Keras`  
  - `Numpy`, `Pillow`  
  - `RPi.GPIO`, `smtplib`, `os`, `time`  
  - `Google Drive API`, `SMSChef API`

---

## 🔄System Workflow

1. **Detection Phase**:  
   Ultrasonic sensor detects movement.

2. **Image Capture**:  
   USB camera captures an image when movement is detected.

3. **Processing Phase**:  
   Image is resized and normalized.

4. **Animal Detection**:  
   CNN model classifies the image into one of 32 animal classes.

5. **Alert System**:  
   SMS alert is sent with date and time of detection.

6. **Cloud Upload**:  
   Captured image is uploaded to a designated Google Drive folder.

---

##  Model Information

- **Model Architecture**: VGG19 with custom dense layers.
- **Accuracy**: Achieved ~92% after training for 100 epochs.
- **Dataset**: 32 animal categories; manually curated and trained.

---

##  Features

- Real-time detection and notification
- Remote monitoring via SSH and Remote Desktop
- Environmentally friendly and low-power
- Cost-effective and scalable
- Fully automated with minimal human intervention

---

##  Future Improvements

- Integrating GPS for location tracking
- Night vision / thermal imaging support
- Multi-sensor detection (PIR, IR, acoustic)
- Expanding the dataset for better model accuracy

---

##  Sample Drive Uploads

Captured images can be accessed [here](https://drive.google.com/drive/folders/1KpIDOjUb-wzxb2SIBHerYpE70AVR6wB-?usp=drive_link)

---



##  Contact

For queries or collaboration:  
**Nallamothu Balakrishna**  
Email: balakrishnanallamothu04@gmail.com
NIT Puducherry


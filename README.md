# Real-Time Emotion Recognition System

A deep learning system that detects human emotions in real-time using webcam feed, built with TensorFlow/Keras and OpenCV.

## 📌 Features
- Real-time face detection using Haar Cascades
- 7 emotion classification (Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral)
- Webcam integration for Google Colab
- Model saving/loading functionality
- Clean, modular Python implementation

## 🗂️ Dataset Information

### FER-2013 Dataset
This project uses the **FER-2013 (Facial Expression Recognition 2013)** dataset from Kaggle.
Link : https://www.kaggle.com/datasets/msambare/fer2013

**Dataset Characteristics**:
- **Total Images**: 35,887
- **Format**: 48×48 pixel grayscale images
- **Classes**: 7 emotions
- **Split**:
  - Training: 28,709 images
  - Public Test: 3,589 images
  - Private Test: 3,589 images

**Class Distribution**:
| Emotion    | Count | Percentage |
|------------|-------|------------|
| Angry      | 4,993 | 13.9%      |
| Disgust    | 547   | 1.5%       |
| Fear       | 5,121 | 14.3%      |
| Happy      | 8,989 | 25.0%      |
| Sad        | 6,077 | 16.9%      |
| Surprise   | 4,002 | 11.2%      |
| Neutral    | 6,198 | 17.3%      |

*Note: Class imbalance is present (especially for Disgust), which should be addressed during training.*

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/tahangz/emotion-recognition.git
cd emotion-recognition
```
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 conv2d (Conv2D)             (None, 46, 46, 32)        320       
                                                                 
 max_pooling2d (MaxPooling2D  (None, 23, 23, 32)       0         
 )                                                               
                                                                 
 dropout (Dropout)           (None, 23, 23, 32)        0         
                                                                 
 conv2d_1 (Conv2D)           (None, 21, 21, 64)        18496     
                                                                 
 max_pooling2d_1 (MaxPooling  (None, 10, 10, 64)       0         
 2D)                                                             
                                                                 
 dropout_1 (Dropout)         (None, 10, 10, 64)        0         
                                                                 
 conv2d_2 (Conv2D)           (None, 8, 8, 128)         73856     
                                                                 
 max_pooling2d_2 (MaxPooling  (None, 4, 4, 128)        0         
 2D)                                                             
                                                                 
 dropout_2 (Dropout)         (None, 4, 4, 128)         0         
                                                                 
 flatten (Flatten)           (None, 2048)              0         
                                                                 
 dense (Dense)               (None, 512)               1049088   
                                                                 
 dropout_3 (Dropout)         (None, 512)               0         
                                                                 
 dense_1 (Dense)             (None, 7)                 3591      
                                                                 
=================================================================
Total params: 1,145,351
Trainable params: 1,145,351
Non-trainable params: 0
_________________________________________________________________

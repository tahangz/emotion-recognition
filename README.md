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

# Audio Deep Fake Detector using CNNs
CNN based deepfake detection model to classify and detect deepfake audio with 85% accuracy. 

Created as a part of the 'Audio Classification and Signal Processing using Deep Learning' project under EEA, IIT Kanpur in Jan'25.

-Engineered a deep learning pipeline using CNNs and RNNs to classify and detect deepfake audio, achieving >80% accuracy.
– Conducted in-depth feature extraction, leveraging MFCCs and chroma features to enhance model robustness against noise and variations in speech patterns.
– Optimized hyperparameters and network architectures to improve classification performance, achieving a balance between precision and recall.

### Description of Dataset- ASVspoof 2021

## Model Description:
CNN Model Architecture
 Feature Extraction:
Conv2D (32, 3×3, ReLU): Detects patterns in the Mel spectrogram.
MaxPooling (2×2): Reduces spatial dimensions.
Conv2D (64, 3×3, ReLU) + MaxPooling: Extracts deeper features.
Flattening & Fully Connected Layers:
Flatten(): Converts 2D features to 1D.
Dense (128, ReLU) + Dropout (50%): Prevents
overfitting and learns high-level features.
Output Layer:
Dense(NUM_CLASSES, Softmax): Classifies audio as real or deepfake

## Results:
Confusion Matrix- 
TP = 6947
FN = 1982
FP = 11
IN = 1060

Accuracy = 80.07%
Precision = 0.9984
Recall = 0.778
F1-score = 0.88
Specificity = 0.99
Type-1 errors = 0.011
Type-2 errors = 0.22

_______________________________________________________

## Files:
deepfake-detector.ipynb : Jupyter notebook code of the model
Deepfake detection.pdf: End term evaluation presentation pdf. 

## Details:
Samarth Sharma Bhardwaj, samarthsb23@iitk.ac.in   
Project done under-
EEA, IIT Kanpur
Dec'24-Feb'25

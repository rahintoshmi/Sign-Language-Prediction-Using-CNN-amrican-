I developed this project to recognize hand signs using deep learning, specifically a Convolutional Neural Network (CNN). It focuses on American Sign Language (ASL) recognition and lays the groundwork for integrating Bangla Sign Language (BSL) in the future. 
Dataset 
Source: [ASL Alphabet Dataset](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) 
Size: 87,000 images (200x200 pixels) 
Classes: 29 total (A-Z, SPACE, DELETE, NOTHING) 
Preprocessing: Resized images to 50x50 pixels for better computational efficiency 
Model Architecture 
Input: 50x50 RGB images 
CNN Layers: 
•	Conv2D (32, 64, 128 filters) with (3,3) kernel sizes 
•	BatchNormalization for stable training 
•	MaxPooling2D (5,5) to reduce spatial dimensions 
•	Dropout (20-40%) to prevent overfitting 
•	Fully Connected Layers: 
•	Flatten
•	Dense (128 neurons, ReLU activation) 
•	Final Output Layer with softmax activation (27 classes) 
Model Performance 
•	Training Accuracy: 68.46% 
•	Validation Accuracy: 74.65% 
•	Loss: 0.8198 (train), 1.9950 (validation) 

Future Improvements 
1. Fine-tuning hyperparameters to improve accuracy 
2. Integrating Bangla Sign Language (BSL) dataset for multilingual sign recognition 
3. Adding real-time sign detection using OpenCV for live hand gesture recognition 
This project is an exciting step toward building AI-powered sign language translation. Feel free to contribute or share feedback! 



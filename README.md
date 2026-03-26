# Handwritten-Digit-Classification-ANN-vs-CNN-

Project Objective

This project aims to build and compare two deep learning models:

✨ Artificial Neural Network (ANN)
✨ Convolutional Neural Network (CNN)

----
🔍 Comparison based on:

 Accuracy
Training Speed
Learning Behavior

----

📂 Dataset Details
 Dataset: MNIST
Total Images: 70,000
Training: 60,000
Testing: 10,000
Image Size: 28 × 28 pixels (Grayscale)

----
⚙️ Tech Stack

Python
TensorFlow / Keras
NumPy
Matplotlib

----
🧠 Model Architectures
  🔷 ANN (Artificial Neural Network)

    Input: Flattened Image (784 features)
    
    Flatten → Dense(128, ReLU) → Dense(64, ReLU) → Dense(10, Softmax)
    
    🔹 Treats image as numeric data
    🔹 Faster training
    🔹 Lower accuracy compared to CNN

  🔷 CNN (Convolutional Neural Network)

     Input: Image (28 × 28 × 1)
    
    Conv2D → MaxPooling → Conv2D → MaxPooling → Flatten → Dense → Output
    
    🔹 Captures spatial features
    🔹 Learns edges, shapes automatically
    🔹 Higher accuracy
----
🔄 Data Preprocessing

✔ Normalize pixel values → (0–255 → 0–1)
✔ Reshape data:
ANN → Flattened
CNN → 4D input (samples, height, width, channel)

----
📊 Results Comparison

Accuracy	- ANN -  95–97%	 CNN - 98–99%
Training Time	Faster	Slower
Learning	Moderate	Strong

----
📈 Learning Behavior

    ANN:
    
    Gradual improvement
    Slightly unstable

    CNN:
    
    Smooth learning curve
    Higher final accuracy

----
🔍 Key Insights

    ANN:
    
    Loses spatial information
    Treats image as flat data
    
     CNN:
    
    Preserves spatial structure
    Extracts features automatically 

  ----
✅ Final Conclusion

   CNN is better for image classification because:

    It understands image structure
    It captures patterns like edges and shapes
    It provides higher accuracy

  ANN is still useful for:
  
    Tabular data
    Simple classification problems

# Persian-License-Plate-Recognition-Using-Hybrid-Classifiers
End-to-end pipeline for detecting, segmenting, and recognizing Persian alphanumeric characters on vehicle license plates using classical computer vision and machine learning techniques.

📌 Project Overview
This project implements a complete license plate recognition system without deep learning. It processes high-resolution vehicle images to extract plates, isolate characters, and classify them using classical ML models. The focus is on Persian (Iranian) license plates.

🚦 Key Components
📐 Plate Detection & Preprocessing
Parsed XML annotations to locate license plates in 1280×1280 images.

Applied edge detection, morphological ops, and Hough transforms to correct skew and remove background noise.

🔳 Character Segmentation
Converted plate crops to grayscale, followed by adaptive thresholding.

Applied connected-component analysis and morphology to isolate characters.

Resized characters to 28×28 patches for consistency.

🤖 Model Training & Prediction
Trained Decision Tree and SVM classifiers on extracted characters.

Used PCA for dimensionality reduction.

Tuned hyperparameters via grid search.

Performed ensemble prediction via majority voting with confidence filtering.

📈 Evaluation
Metrics: Precision, Recall, Accuracy, and Confusion Matrix.

Evaluated at both character-level and plate-level.

Achieved high performance on real-world test data.


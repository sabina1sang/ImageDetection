🐶🐱 Dog vs Cat Image Classifier
This project uses a Convolutional Neural Network (CNN) to classify 100x100 RGB images as either dog or cat. The model is trained using TensorFlow/Keras and includes data preprocessing, training, evaluation, and prediction visualization.

🧠 Model Summary
Architecture: Simple CNN with:

Two convolutional layers

Max pooling

Fully connected (dense) layers

Loss Function: Binary Crossentropy

Optimizer: Adam

Input Image Size: 100x100x3 (RGB)

Output: Binary label (0 = dog, 1 = cat)

📁 Dataset Files Required
Place the following CSV files in the root directory:

input.csv – Training image data (flattened)

labels.csv – Training labels (0 or 1)

input_test.csv – Testing image data (flattened)

labels_test.csv – Testing labels (0 or 1)

Each image should be flattened to a row of 30,000 pixels (100x100x3) in the CSV files.

🚀 Getting Started
1. Install Dependencies
bash
Copy
Edit
pip install numpy matplotlib tensorflow gradio opencv-python
2. Run the Script
bash
Copy
Edit
python your_script_name.py
📊 Training & Evaluation
The script:

Loads and reshapes the CSV data into image tensors.

Normalizes the images.

Trains a CNN for 5 epochs.

Evaluates accuracy on the test set.

Shows a sample prediction.

🖼️ Visualization
During training and evaluation, a random image is shown using matplotlib to give visual context to predictions.

🤖 Model Prediction
A single test image is randomly chosen and predicted:

If prediction > 0.5514 → Cat

Else → Dog

Prediction output is printed to the console.

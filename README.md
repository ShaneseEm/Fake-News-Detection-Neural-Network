# Fake News Detection Using a Neural Network

This repository contains a deep learning project that classifies news headlines as either **Real** or **Fake**. This project was developed to apply concepts of neural network architecture, activation functions, and text preprocessing.

##  Project Overview
- **Goal**: Build a text classification model to predict news authenticity.
- **Dataset**: WELFake Dataset (0 = Real News, 1 = Fake News).
- **Tool**: Python, TensorFlow/Keras, and Scikit-learn.

##  Project Workflow
1. **Data Loading**: Used Pandas to read and explore the news samples.
2. **Preprocessing**: Converted raw text into numerical vectors using **TF-IDF Vectorization**.
3. **Data Splitting**: Divided data into 80% training and 20% testing sets.
4. **Model Architecture**: Built a Feedforward Neural Network with two hidden layers.
5. **Training**: Trained for 15 epochs using the Adam optimizer and Binary Crossentropy loss.
6. **Evaluation**: Assessed performance on unseen test data.

##  Neural Network Architecture
The model follows a Sequential architecture:
- **Input Layer**: 5,000 features (TF-IDF).
- **Hidden Layer 1**: 128 neurons with **ReLU** activation.
- **Hidden Layer 2**: 64 neurons with **ReLU** activation.
- **Output Layer**: 1 neuron with **Sigmoid** activation.

##  Deliverables & Results
- **Model Accuracy**: [Insert your Accuracy from Step 6 here, e.g., 94.2%]
- **Model Loss**: [Insert your Loss from Step 6 here]
- **Trained Model**: Available in the `/models/` folder.
- **Notebook**: View the [Kaggle Notebook](https://www.kaggle.com/code/bethelhemalemayehu/fake-news-detection-nn/edit).

### Assignment Questions
* **Architecture**: Feedforward Neural Network (Input -> 128 -> 64 -> Output).
* **Epochs**: 15.
* **Activation Functions**: ReLU for hidden layers; Sigmoid for the output layer.
* **Accuracy**: [Insert your Accuracy here].

##  Manual Testing Examples
| Headline | Prediction |
| :--- | :--- |
| "Scientists confirm water on Mars." | **Real News** |
| "Secret government project creates invisible humans." | **Fake News** |

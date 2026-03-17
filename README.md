# Fake News Detection Using a Neural Network

This repository contains a deep learning project designed to classify news headlines as either **Real** or **Fake**. The project implements a Feedforward Neural Network (FNN) using TensorFlow and Keras to identify patterns in labeled news data.

##  Project Overview
- **Objective**: Build a text classification model to predict news authenticity based on headlines.
- **Dataset**: [WELFake Dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification) containing 72,134 news samples.
- **Labels**: 0 = Real News, 1 = Fake News.
- **Tools**: Python, TensorFlow/Keras, Scikit-learn, and Pandas.

##  Repository Structure
- `notebooks/`: Contains the full implementation in `fake-news-detection-nn.ipynb`.
- `models/`: Contains the trained and saved model file `fake_news_model.h5`.
- `README.md`: Project documentation and summarized results.

##  Project Workflow
1. **Data Loading**: Used Pandas to read the dataset and performed initial exploration of the samples.
2. **Preprocessing**: Converted raw text headlines into numerical vectors using **TF-IDF Vectorization** with 5,000 features.
3. **Data Splitting**: Divided the dataset into **80% training** and **20% testing** sets.
4. **Model Architecture**: Designed a Feedforward Neural Network with two hidden layers.
5. **Training**: Trained the model for **15 epochs** using the Adam optimizer and Binary Crossentropy loss.
6. **Evaluation**: Tested the model performance on unseen data to calculate accuracy and loss.
7. **Manual Testing**: Implemented a function to predict labels for new, unseen headlines.

##  Neural Network Architecture

The model follows a Sequential architecture:
- **Input Layer**: 5,000 features (derived from TF-IDF).
- **Hidden Layer 1**: 128 neurons with **ReLU** activation.
- **Hidden Layer 2**: 64 neurons with **ReLU** activation.
- **Output Layer**: 1 neuron with **Sigmoid** activation for binary probability.

##  Performance Results
- **Final Test Accuracy**: **90.60%**.
- **Final Test Loss**: **0.9122**.
- **Training Epochs**: 15.
- **Optimizer**: Adam (Learning Rate: 0.001).

##  Assignment Deliverables
* **Architecture**: Feedforward Neural Network (Input -> 128 -> 64 -> Output).
* **Epochs**: 15.
* **Activation Functions**: **ReLU** for hidden layers and **Sigmoid** for the output layer.
* **Accuracy Achieved**: **90.60%**.

##  Manual Testing Examples
| Headline | Model Prediction |
| :--- | :--- |
| "Scientists confirm water on Mars." | **Fake News*** |
| "Secret government project creates invisible humans." | **Fake News** |

*\*Note: Short headlines may be classified as Fake depending on the TF-IDF vocabulary weights learned from the training data. Performance can be further enhanced using word embeddings.*

## 🔗 Links
- **Kaggle Notebook**: [View Notebook on Kaggle](https://www.kaggle.com/code/bethelhemalemayehu/fake-news-detection-nn/edit).

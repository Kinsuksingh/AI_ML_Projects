# AI and Machine Learning Projects

Welcome to my AI and Machine Learning project repository! This repository showcases two projects: a **Speech Assistant** powered by Google GenAI and **Heart Disease Prediction** using Logistic Regression.

---

## Projects Overview

1. **Speech Assistant**
   - A voice-activated assistant that takes audio input, converts it to text, generates a response using Google GenAI, and finally reads the response aloud.
   - **Core Features**:
     - Converts audio commands into text.
     - Integrates Google GenAI for intelligent response generation.
     - Text-to-speech functionality for a conversational experience.
   - **Libraries Used**: `speech_recognition`, `pyttsx3`, `google.generativeai`
   - **APIs Used**: Google Generative AI

2. **Heart Disease Prediction**
   - A logistic regression model to predict the likelihood of heart disease based on various medical factors.
   - **Core Features**:
     - Uses logistic regression for classification.
     - Predicts whether a patient is likely to have heart disease based on their medical data.
     - Trains on data and evaluates model accuracy using test data.
   - **Libraries Used**: `numpy`, `pandas`, `sklearn`

---

## 1. Speech Assistant

### How It Works
The Speech Assistant follows this workflow:
1. **Capture Audio Command**: Listens to a voice command through the microphone.
2. **Convert Speech to Text**: Transforms the spoken command into text using `speech_recognition`.
3. **Generate AI Response**: Sends the text command to Google GenAI and receives a generated response.
4. **Text-to-Speech**: Uses `pyttsx3` to convert the AI-generated response back to speech and read it aloud to the user.

### Code Overview
The main functions in this project include:
- `Reply(question)`: Connects to Google GenAI and retrieves a response.
- `speak(text)`: Reads out any text provided as input using `pyttsx3`.
- `takeCommand()`: Listens for and processes the user's spoken command.

### Example Output
- **User says**: "What's the weather today?"
- **Assistant replies**: "Today's weather forecast is sunny with a chance of rain in the evening."

### Run the Project
To run the project:
1. Install the required libraries: `speech_recognition`, `pyttsx3`, and `google.generativeai`.
2. Set up your Google GenAI API key.
3. Run the `main.py` file and give voice commands.

---

## 2. Heart Disease Prediction

### How It Works
The Heart Disease Prediction project is based on logistic regression and follows these steps:
1. **Data Processing**: Loads and prepares data, checking for null values and performing exploratory analysis.
2. **Training and Testing**: Splits the data into training and testing sets, using the training set to fit the model.
3. **Evaluation**: Calculates accuracy on both training and testing data for model evaluation.

### Code Overview
The main functions in this project include:
- `model.fit()`: Trains the logistic regression model on the training data.
- `model.predict()`: Predicts the outcomes on test data.
- **Accuracy Calculation**: `accuracy_score()` is used to evaluate model performance.

### Example Output
- **Input Data**: Patient information in a tuple format.
- **Prediction**: "Healthy" (0) or "Heart Disease" (1) based on the model's accuracy.

### Run the Project
To run the project:
1. Install the required libraries: `numpy`, `pandas`, `sklearn`.
2. Load your data in CSV format.
3. Run the script to train the model and make predictions on new data.

---

## Installation and Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Kinsuksingh/AI_ML_Projects.git

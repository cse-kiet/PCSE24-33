# PCSE24-33

# Speech Emotion Recognition

## Overview

Speech Emotion Recognition (SER) is an emerging field in the domain of human-computer interaction. SER involves the recognition of emotions conveyed through speech, utilizing variations in tone, pitch, and intensity. This project aims to harness deep learning techniques to build an accurate and robust SER system capable of identifying different emotional states such as happiness, sadness, anger, and neutrality from audio recordings.

The importance of SER is underscored by its numerous real-world applications:

**Improving Customer Service**: SER can be used in call centers to monitor and classify customer emotions, helping in identifying unsatisfied customers and improving service quality.

**Enhancing Driver Safety**: In-car systems can use SER to detect drivers' emotional states, providing alerts or interventions to prevent accidents.

**Advancing Human-Computer Interaction**: SER can make interactions with virtual assistants and other AI systems more natural and responsive to human emotions.

**Supporting Cognitive and Psychiatric Analysis**: SER can aid in psychiatric assessments and cognitive analysis by providing insights into a person's emotional state.

This project utilizes deep learning models to analyze and interpret emotions from speech, combining and preprocessing audio data from various datasets to extract features effectively. The results demonstrate significant real-world applications and the potential to improve interactions between humans and machines.


## Datasets
This project uses several well-known datasets for training and evaluation:

**RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**:

The RAVDESS dataset contains 24 professional actors (12 male, 12 female) vocalizing two lexically-matched statements in a neutral North American accent. Speech includes calm, happy, sad, angry, fearful, surprise, and disgust expressions.

[*kaggle datasets download -d uwrfkaggler/ravdess-emotional-speech-audio*](url)

**CREMA-D (Crowd-sourced Emotional Multimodal Actors Dataset)**:

The CREMA-D dataset includes 7,442 clips from 91 actors (48 male, 43 female), aged 20 to 74, from different ethnic backgrounds. The actors spoke from a selection of 12 sentences in six different emotions: anger, disgust, fear, happy, neutral, and sad.

[*kaggle datasets download -d ejlok1/cremad*](url)

**TESS (Toronto Emotional Speech Set)**:

The TESS dataset consists of recordings from two actresses (aged 26 and 64 years) who spoke 200 target words in the carrier phrase “Say the word _ again”. The set includes seven emotions: anger, disgust, fear, happiness, pleasant surprise, sadness, and neutral.

[*kaggle datasets download -d ejlok1/toronto-emotional-speech-set-tess*](url)

**SAVEE (Surrey Audio-Visual Expressed Emotion)**:

The SAVEE dataset consists of recordings from four male actors, each delivering 15 sentences in seven different emotions: anger, disgust, fear, happiness, sadness, surprise, and neutral.

[*kaggle datasets download -d ejlok1/surrey-audiovisual-expressed-emotion-savee*](url)

These datasets are combined and preprocessed to extract features such as log-mel spectrograms, which are then used to train deep learning models for emotion recognition. The diversity and quality of these datasets ensure robust model training and evaluation, enhancing the system's performance and accuracy in real-world applications.

## Methodology
The main purpose of SER is to increase human-machine interaction.
**Block Diagram**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/a644f2a1-2685-43a3-813a-2e7e8344bd71)

## Working Model
To begin with, it is crucial to remember that there are 
numerous platforms available for running and executing 
Python code. Several platforms are available, including 
1. Google Colab 
2. Kaggle
3. Pycharm 
4. Jupyter Notebook

##  Preprocessing 
The imported audio files are then pre-processed from the Ravdess, Crema DataFrame, TESS dataset, and SAVEE Dataset.

**INSTANCES AND EMOTIONS**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/08ee367a-296e-47c3-b386-8dfd7beaca84)

**Emotions Graph**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/23865d42-9577-42c6-947b-9b385da47c88)

**Create mel Spectrogram**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/f5c42749-a720-43d9-b2e1-9b490122685c)

## Data Augmentation

**Normal Audio**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/f842dec9-bcf3-49e8-8d49-ff0dc2f33b57)

**Audio with Noise**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/f808d412-0282-4886-aa43-06e79dfba914)

 **Stretched Audio**
 
 ![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/52f8fb6f-5d77-4aac-b10a-63627de22be3)
 
**Shifted Audio**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/72cbf49c-55ca-4b8b-a174-8e768f3c997e)

## Feature Extraction

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/909b3d78-7336-4d61-aeba-07296d7729a4)
![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/4282be4a-d5b5-4932-9b06-adf54db9d75f)

## Prediction the Emotion

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/d0ef816c-7089-4eda-a137-1817b257c565)

It offers a concise summary of the model's performance on the test data. It is making predictions on the test data using a trained model.

## Evaluation

Evaluation ensues, rigorously assessing the performance of different models, and results from the best-performing model are scrutinized based on predefined metrics.

**Confusion Matrix**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/7b38b1c7-10cb-40dc-86b2-899e267e36c8)

**Predicted Labels

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/37bbce77-638a-4975-8cb8-fea01d6c9e65)

## Result Analysis

**Accuracy**

![image](https://github.com/cse-kiet/PCSE24-33/assets/117917432/5e3b05e7-970c-4c6a-9791-8fe6d7193a82)

## Conclusion

Our exploration of Speech Emotion Recognition (SER) demonstrates the effectiveness of using CNN models and log-mel spectrograms for feature extraction on datasets like RAVDESS, CREMA-D, TESS, and SAVEE. The results highlight SER's significance in real-world applications, effectively distinguishing emotional signals in speech. Future research should focus on diverse datasets, novel feature extraction techniques, and interdisciplinary collaborations to further advance SER systems.

Additionally, this repository includes supplementary files such as the research paper, presentation(PPT), certificates as we recieved best paper award, synopsis of the project, and the final project report.

-Presented by Divya Garg,Amrita Singh and Anshika Gupta.

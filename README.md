# DeepSign

Traffic Sign Detection System

## Table of Contents:

- [Background](#Background)
- [Objectives](#Objectives)
- [SDG Relation](#SDG)
	- [Sustainable Cities and Communities](#Sustainable)
	- [Climate Action](#Climate)
- [Dataset](#Dataset)
	- [Feature Engineering](#Feature)
	- [Exploratory Data Analytics](#Exploratory)
- [Methodology](#Methodology)
	- [Model](#Model)
	- [Hyperparameter Tuning](#Hyperparameter)
- [Outputs](#Outputs)
- [Usage](#Usage)
- [Next Steps](#Next)

## Background

- Traffic accidents are a major public health problem, with more than 1.35 million deaths and tens of millions of injuries worldwide each year.
- One of the most important causes of traffic accidents is failure to comply with traffic lights and signs.
- The use of AI for traffic lights and traffic sign detection has the potential to reduce the number of traffic accidents caused by non-compliance.
- These systems can help enforce road rules and prevent collisions by providing real-time information and alerts to drivers. 

## Objectives

- The use of AI for traffic lights and traffic sign detection has the potential to reduce the number of traffic accidents caused by non-compliance.
- The system proposes a new approach based on convolutional neural networks (CNNs) to detect traffic signs in real-time video streams.
- It also presents a case study of its implementation and evaluation in a real-world scenario, and its implications and potential impacts on traffic safety are discussed.

## SDG Relations

- Sustainable Cities and Communities
- Climate Action

## Sustainable Cities and Communities Relation

- The project directly contributes to Sustainable Development Goals, particularly towards Sustainable Cities and Communities by enhancing road safety. 
- Through improved traffic sign detection, we aim to create safer urban environments, promoting better traffic management and reducing road accidents within cities. 

## Climate Action  Relation

- By enabling efficient navigation and adherence to traffic regulations, our system supports Climate Action objectives by potentially reducing traffic congestions and subsequently lowering vehicle emissions, contributing to a cleaner and greener environment.

## Datasets
- [The German Traffic Sign Recognition Benchmark (GTSRB)](http://benchmark.ini.rub.de/2)<br> is a widely used dataset for traffic sign recognition. It consists of more than 50,000 images of traffic signs, including speed limit signs, stop signs, and warning signs. 
	- 42 Class
	- 541 Images
	- 23000 Images Total

## Metadology
- Models
	- KoLNet
	- EfficientNet
	- Resnet

## KoLNet
- Compilation Time: 218 sec
- Accuracy: 0.989

| Epoch | s   | ms/step | Loss   | Accuracy | Validation Loss | Validation Accuracy |
|-------|-----|---------|--------|----------|-----------------|---------------------|
| 1     | 23  | 97      | 2.6114 | 0.2628   | 1.6327          |                     |
| 2     | 22  | 102     | 1.0087 | 0.7027   | 0.5831          |                     |
| 3     | 23  | 106     | 0.4081 | 0.8899   | 0.2704          |                     |
| 4     | 21  | 97      | 0.219  | 0.9466   | 0.1709          |                     |
| 5     | 21  | 96      | 0.134  | 0.9698   | 0.1083          |                     |
| 6     | 21  | 96      | 0.0901 | 0.9794   | 0.1096          |                     |
| 7     | 21  | 95      | 0.698  | 0.9827   | 0.685           |                     |
| 8     | 22  | 101     | 0.0507 | 0.9882   | 0.0701          |                     |
| 9     | 23  | 104     | 0.348  | 0.9923   | 0.0582          |                     |
| 10    | 21  | 95      | 0.0263 | 0.9941   | 0.0484          |                     |

## EfficientNet
- Compilation Time: 12 min
- Accuracy: 0.928

## ResNet
- Compilation Time: 235 min
- Accuracy: 0.953

## Next Step
- This project aims to comparing the models between popular models and KoLNet to create better model.
- The next step is to detect traffic signs in video images or live images and warn the user.



















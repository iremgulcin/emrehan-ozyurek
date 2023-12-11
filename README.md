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
- Compilation Time: 23 min (1389 sec)
- Accuracy: 0.952

| Epoch | s   | ms/step | Loss   | Accuracy | Validation Loss | Validation Accuracy |
|-------|-----|---------|--------|----------|-----------------|---------------------|
| 1     | 165 | 631     | 3.3281 | 0.2048   | 3.188           |                     |
| 2     | 136 | 625     | 1.9958 | 0.4536   | 3.1216          |                     |
| 3     | 136 | 625     | 1.2687 | 0.6436   | 1.9487          |                     |
| 4     | 139 | 637     | 0.8882 | 0.7521   | 0.6915          |                     |
| 5     | 137 | 627     | 0.5743 | 0.828    | 0.4958          |                     |
| 6     | 132 | 603     | 0.4397 | 0.8769   | 0.5922          |                     |
| 7     | 137 | 627     | 0.3058 | 0.9094   | 0.2902          |                     |
| 8     | 137 | 627     | 0.223  | 0.9305   | 0.2111          |                     |
| 9     | 134 | 615     | 0.1845 | 0.9431   | 0.2895          |                     |
| 10    | 136 | 622     | 0.1534 | 0.9515   | 0.1973          |                     |

## ResNet
- Compilation Time: 175 min (10424 sec)
- Accuracy: 0.937

| Epoch | s    | s/step | Loss   | Accuracy | Validation Loss | Validation Accuracy |
|-------|------|--------|--------|----------|-----------------|---------------------|
| 1     | 1079 | 5      | 2.2902 | 0.3796   | 3.5454          |                     |
| 2     | 1041 | 5      | 0.7119 | 0.7986   | 2.3891          |                     |
| 3     | 1044 | 5      | 0.2963 | 0.9142   | 0.344           |                     |
| 4     | 1037 | 5      | 0.4911 | 0.8725   | 0.4314          |                     |
| 5     | 1021 | 5      | 0.1912 | 0.9512   | 14.8984         |                     |
| 6     | 1014 | 5      | 0.4041 | 0.8902   | 1.4258          |                     |
| 7     | 1048 | 5      | 0.1998 | 0.9596   | 0.1023          |                     |
| 8     | 1057 | 5      | 0.0849 | 0.9838   | 0.0863          |                     |
| 9     | 1047 | 5      | 0.1601 | 0.9686   | 0.4512          |                     |
| 10    | 1036 | 5      | 0.2985 | 0.9369   | 0.9715          |                     |

## Next Step
- This project aims to comparing the models between popular models and KoLNet to create better model.
- The next step is to detect traffic signs in video images or live images and warn the user.



















# Project Vision

A Django powered API endpoint for our project.

Project Vision
Introduction
Surveillance means safety. Despite so much surveillance, the crime rates are increasing. The problem lies in the fact that inspecting several hundreds and thousands of videos is very laborous and time-intensive task. Only after a crime is committed, these footages are inspected to find the crime scenes evidence, which proves to be highly inefficient considering the massive amount of footages. This manual task provides evidence in court but is rarely used to prevent crime or react to it in real-time.


🔭   About this Project
In this project, we aim to develop a real-time crime detection technology that can be integrated with any security system, to ensure public safety through visual crowd surveillance.
We have devised a complete software solution for safety and surveillance where we convert these CCTVs from an evidence collection to a crime prevention and detection tool to ensure safety and security.
This real-time crime detection technology is integrated with security systems and Desktop Application to get push-in notifications in case any suspicious activity is discovered. The system will detect and simultaneously alert any violent activity captured by the camera.
The technologies encompasses domains of Computer Vision and Deep Learning models like CNN, R-CNN, LSTM. The dataset consists of 500+ videos scraped off internet and categorized into violent and non-violent activities.

🛠  Tech Stack
Tensorflow  Keras  Django  Node.js 
AWS  Python  HTML  CSS  Javascipt

💼   Testing
Our source code can be tested and contributed to using the following steps:

1. Website
Execute the following sequence of code to start contributing and testing:

Open the directory labelled Website using the command

cd Website
Install all the dependencies using

pip3 install -r requirements.txt
Run the migrations using the following commands

python3 manage.py makemigrations
python3 manage.py migrate
Run the Django server by

python3 manage.py runserver

Note : In case you encounter errors during migrations, make sure that you have access rights to db.sqlite3 file. You can use the following command to rectify permission denied error

chown *username* db.sqlite3
Run the migrations again to continue.

2. Desktop App
Being built on top of Node.js, it is fairly easy to set-up the environment. Follow the steps to safely configure the system

From the parent folder directory, execute the following command

npm install
Once finished, the application can be run using

npm start
The desktop app has two modes of operation: Offline and Online. By default the app function in Online mode. To make it work in Offline mode, use the menu button provided on top of UI and select Offline mode.






✍️   Current Progress
We tried and tested various architectures for this project. A brief summary and stats for each is given below:

Customised CNN Model: The customised CNN model with optimised parameters performed well on the training and sufficiently good in the test dataset. The architecture is currently being used by the website and test.ipynb file.

Accuracy on training: 0.7990
Loss on training: 0.4292
Val_loss: 0.7605
Val_accuracy: 0.6680
Optimizer: Adam
Loss: BinaryCrossEntropy
Epochs: 50
steps_per_epoch: 50





VGG Net: VGGNet Architecture displayed an accuracy of 60% on training and 55% on testing dataset.

Testing Accuracy: 0.5513





AlexNet: AlexNet showed accuracy of 57% on training and a similar accuracy on the testing dataset.

Testing Accuracy: 0.5729






Inception+CustomisedCNN: Using transfer learning of Inception Architecture and passing it to CustomisedCNN trained the model with satisfactory results.

Training_accuracy: 89%
Validation_accuracy: 76%
Epochs: 30
Steps per Epoch: 100
Optimizer: RMSprop with LR 0.0001
Loss: Binarycrossentropy




⚙️   Ultimate Objective
The model uses the technique of Multiple Object Detection with Localization tracking the movement of people and then categorizing it into violent or non-violent behavior. Our proposed solution will ensure Public Safety and security without any human toil with an instant alert to the concerned authorities. Through Crowd Monitoring and Behavioral Analysis our solution aims to evoke the sense of security in men and women. The constant rise of criminal activities, their unexpectedness, and scope of harm that can be inflicted can be exponentially reduced through our proposed system.

Link to current protoytpe : Click Here

Link to Desktop Apps
Platform   	      Link     
Windows (.exe)	      Link
Linux (.AppImage)                               	      Link
Mac (.dmg)	      Link

Custom Build
If you want to create the desktop app for a different platform or a different extension like .deb, .rpm, use the following command from parent folder

electron-forge make

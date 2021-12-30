[![CircleCI](https://circleci.com/gh/InaArya/ML_Project4/tree/main.svg?style=svg)](https://circleci.com/gh/InaArya/ML_Project4/tree/main)

## Overview

The projetct deploys an application to predict minimum prices of houses in Bouston. The projects uses Python based app, Docker container and Kubernetes for the orchestration of the container. The tasks like generating logs from python script, Docker image creation and Kubernetes minikube usages are part of the project.

### How to run the Python scripts

First, Docker account should be created and an image needs to be create. Second, minikube should be installed.

Below are the specific commands:
I worked on Mac system, so below are the Mac specific commands i used for this project.

1. Create and activate Python environment:

python3 -m venv ~/.devops
source ~/.devops/bin/activate

2. Install VirtualBox:

brew cask install virtualbox

3. Install minikube & start:

brew cask install minikube

4. Start minikube
minikube start

5. Run Docker file
./run_Docker.sh

4. Run prediction file
./make_Prediction.sh

5. Run Kubernetes file

./run_kubernetes.sh

On a separate tab, call the script to make prediction.
./make_prediction2.sh

Once done,delete the minikube
minikube delete


## Files in Repository
.circleci/congif.yml - config file for integration of application with circleci
DockerFile - Required file to Dockerize the python app
MakeFile - File which keeps commands for installations
README.md - File which keeps info about the project
app.py - Phython file which contains data about making predictions
make_predictions.sh - Performs a call to the API to perform prediction
requirements.txt - This file keeps a list of all the dependency required for the project
run_docker.sh - Required to run the docker container
run_kubernetes.sh - Runs the Kubernetes container
upload_docker.sh - This file uploads the docker file to Docker Hub
model_data - Folder contains the sample input data for making predictions
output_txt_files - Folder contains the log info which is captured at different stages of project


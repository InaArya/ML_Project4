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

Start minikube
minikube start

4. Run Docker file
./run_Docker.sh

4. Run prediction file
./make_Prediction.sh

5. Run Kubernetes file
Run Kubernetes
./run_kubernetes.sh
On a separate tab, call the script to make prediction.
./make_prediction2.sh
Once done,delete the minikube
minikube delete


## Files in Repository



### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Vanbliser/DevOps_Microservices/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Vanbliser/DevOps_Microservices/tree/main)

## Project Overview

In this project, I apply the skills I have acquired in this course to operationalize a Machine Learning Microservice API. 

I was given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

My project goal was to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project I:
* Tested my project code using linting
* Completed a Dockerfile to containerize this application
* Deployed a containerized application using Docker and make a prediction
* Improved the log statements in the source code for this application
* Configured Kubernetes and created a Kubernetes cluster
* Deployed a container using Kubernetes and make a prediction
* Uploaded a complete Github repo with CircleCI to indicate that your code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

---

** Ensure that the following are installed **

* Docker
* Hadolint
* Kubernetes (Minikube)
* 

## Instructions on how to run the Python scripts and web app

* Create a virtul enviroonment `python3 -m venv ~/.devops` and activate it `source ~/.devops/bin/activate`. Run `make setup`
* Install dependencies `make install` The Makefile contains logic to properly install dependencies listed is the requirements.txt file amongst other things
* Create container by editing the Dockerfile. Then run `bash run_docker.sh` to run the container
* Make Prediction by running `bash make_prediction.sh`. 
* To upload your Image run `bash upload_docker.sh`
* To run kubernetes, run `bash run_kubernetes.sh`


## A short explanation of the files in the repository.

* Output_txt_files: Contains text files of outputs gotten from the tasks
* Dockerfile: A file docker uses to build images/containers
* make_prediction: A script to make predictions
* Makefile: A file used by `make` to run commands
* requirements.txt: A file used by pip to install project dependencies (packages)
* run_docker: A script to create and run docker container
* run_kubernetes: A script to run kubernetes
* upload_docker: A script to push your docker container/image to DockerHub


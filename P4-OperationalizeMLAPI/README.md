[![CircleCI](https://circleci.com/gh/nevermyuk/project-ml-microservice-kubernetes.svg?style=svg)](https://circleci.com/gh/nevermyuk/project-ml-microservice-kubernetes)
## Project Overview

Oerationalized Machine Learning Microservice API. 
A pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. 
Python Flask app serves out predictions (inference) about housing prices through API calls.
This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.


## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`

2. Run in Docker:  `./run_docker.sh` 


#### Kubernetes Steps
1. `./run_docker.sh` to build image.
2. `./upload_docker.sh to upload image to docker hub.
3. Run in Kubernetes:  `./run_kubernetes.sh`


### Calling the API
1. Run `./make_prediction.sh` to call the API.

### How it works

- Makefile -  Build automation.
- App.py - Flask App to return API calls.
- Dockerfile - Creation of Docker Image
- requirements.txt - for dependencies
- .circleci - For CI
- deployment.yaml for Kubernetes Deployment configuration


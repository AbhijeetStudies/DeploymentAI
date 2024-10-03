# DeploymentAI

## Overview

This project is a simple machine learning application that uses Flask and Docker to serve predictions based on the Iris dataset. A decision tree classifier is trained on the dataset, and the model is deployed using a Flask web application. The application allows users to make predictions through a RESTful API.

## Project Structure


## Instructions to Build and Run the Docker Container

1. **Clone the Repository**

   Clone this repository to your local machine:

   ```bash
   git clone https://github.com/AbhijeetStudies/DeploymentAI.git
   cd DeploymentAI
Build Docker Container:
   docker build -t deploymentai .
   docker run -p 80:80 deploymentai

Instruction to Test the ML endpoint

curl -X POST http://localhost/predict -H "Content-Type: application/json" -d '{"input": [5.1, 3.5, 1.4, 0.2]}'

You should receive a response indicating the predicted class:

json

{"prediction":0}

[![CircleCI](https://circleci.com/gh/acserna/Operationalize-ML-Microservice-API.svg?style=svg)](https://circleci.com/gh/acserna/Operationalize-ML-Microservice-API)

# Summary
In this project, I could operationalize a Machine Learning Microservice API (developed in flask) to predict the price of certain house through API calls. I create the container and the deployment configuration to kubernetes, all of it developing and executing lint tests using the Makefile.

# Setup the environment
- Run "make setup" to create a virtualenv
- Activate the virtualenv with "source ./.devops/bin/activate"
- Run "make install" to install the necessary dependencies
- Run "make lint" to run lint checks on the project code

# Run in Docker: 
  ./run_docker.sh

# Upload docker image to dockerhub
  ./upload_docker.sh

# Run in Kubernetes:
  ./run_kubernetes.sh, you need a kubernetes server
  
# Make prediction
  ./make_prediction.sh

The pretrained model is located in "model_data/boston_housing_prediction.joblib"

All the development of the project was realized in Cloud9 from AWS.

## Project Description

The project deploys a sentiment analysis web app, trained using an XGBoost Classifier, within AWS ecosystem.

Project Steps:
1. Train a model for sentiment analysis using XGBoost classifier in Sagemaker.
2. Create a sagemaker endpoint to send inputs to the trained model.
3. Since sagemaker endpoint is only accessible from within AWS services (for which we need to explicitly grant the permission to the service), we will create an API using API Gateway service which will call the sagemaker API.
4. We also need to process the inputs before passing it to the model, therefore we use Lambda function, which will process the input and pass it to the model.
5. We can then expose the API created through the API Gateway to the client to use the web app.

#### AWS Services Used : Sagemaker, API Gateway, Lambda, S3


Note: App not available for demo since it is kinda expensive to keep a Sagemaker endpoint running.

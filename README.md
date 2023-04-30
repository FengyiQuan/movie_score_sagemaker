## Movie score predictor

Welcome to my project, a movie score predictor using Amazon SageMaker, API Gateway, and Amazon S3. In this project, I
have developed a machine learning model that predicts the score of a movie based on its various features such as
director, genre, and cast. The model has been trained on a dataset containing information about thousands of movies and
their respective scores.

To deploy the model, I have used Amazon SageMaker, a fully-managed machine learning service provided by Amazon Web
Services (AWS). With SageMaker, I have been able to create and manage machine learning models using built-in algorithms,
custom algorithms, and my own training code.

The model is deployed using an API Gateway, which provides a RESTful interface for accessing the model. The API Gateway
is integrated with Amazon S3, a highly scalable and durable object storage service provided by AWS, which stores the
model's input and output data.

Overall, this project demonstrates how powerful machine learning tools such as Amazon SageMaker, API Gateway, and S3 can
be used to build and deploy sophisticated machine learning models with ease. By predicting the scores of movies, this
project can help movie producers and distributors make informed decisions about the movies they create and distribute.

### Infrastructure

![infrastructure](https://d2908q01vomqb2.cloudfront.net/f1f836cb4ea6efb2a0b1b99f41ad8b103eff4b59/2020/03/04/api-gateway-sagemaker-1.gif)

### SageMaker

Amazon SageMaker is a fully-managed machine learning service provided by Amazon Web Services (AWS). It allows data
scientists and developers to build, train, and deploy machine learning models at scale. With SageMaker, users can easily
create and manage machine learning models using built-in algorithms, custom algorithms, and their own training code.

### API Gateway

Amazon API Gateway is a fully managed service provided by Amazon Web Services (AWS) that makes it easy for developers to
create, publish, maintain, monitor, and secure APIs at any scale. It acts as a front door for applications to access
data, logic, or functionality from backend services and applications.

### Usage

https://0rg8yrwjql.execute-api.us-east-1.amazonaws.com/test/predicted-ratings/321?items=101,131,162&

### Inheritance

https://aws.amazon.com/blogs/machine-learning/creating-a-machine-learning-powered-rest-api-with-amazon-api-gateway-mapping-templates-and-amazon-sagemaker/
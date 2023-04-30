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

### S3

Amazon S3 (Simple Storage Service) is a highly scalable, secure, and durable object storage service provided by Amazon
Web Services (AWS). It allows users to store and retrieve any amount of data from anywhere on the web. S3 provides
object-level storage, which means that data is stored in objects, such as files or images, within buckets. A bucket is a
container for objects, similar to a folder in a file system.¬

### Dataset

http://files.grouplens.org/datasets/movielens/ml-100k.zip

### Model

It presents a scenario where a television application seeks to obtain forecasted ratings for a selection of films. When
the application presents a page of movies to the user, it should prioritize the display of those movies with higher
ratings predictions, making them more visible on the page. The scenario assumes that both users and movies are
distinguishable by a numerical ID, and the predicted ratings are on a scale ranging from 1 to 5. A higher rating
indicates a greater probability that a specific movie will be enjoyed by the user.

This prediction model has the capability to predict the score of a movie based on the user's individual preferences.
Essentially, the model is able to analyze a user's past behavior and movie preferences to determine the likelihood that
they will enjoy a particular movie. By utilizing this user-based approach, the model can provide personalized
recommendations to each user, which can lead to a more satisfying and enjoyable movie-watching experience. This type of
personalized prediction model is becoming increasingly popular in the entertainment industry, as it allows companies to
tailor their services to each individual user's preferences, ultimately leading to increased customer satisfaction and
loyalty.

### Usage

https://0rg8yrwjql.execute-api.us-east-1.amazonaws.com/test/predicted-ratings/321?items=101,131,162&

```bash
curl "https://0rg8yrwjql.execute-api.us-east-1.amazonaws.com/test/predicted-ratings/321?items=101,131,162&"
```

### Inheritance

https://aws.amazon.com/blogs/machine-learning/creating-a-machine-learning-powered-rest-api-with-amazon-api-gateway-mapping-templates-and-amazon-sagemaker/
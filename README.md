# Serverless Twitter Follower Notification Application

This serverless application uses the AWS SAM model and Twitter APIs to notify registered users of any follows or unfollows by a specific Twitter user, ensuring scalability and efficient performance. The application is built using the AWS Serverless Application Model (SAM) and leverages AWS Lambda, API Gateway, and SNS services to provide a scalable and efficient solution.

## How it Works

The application is built using the following AWS services:

- AWS Lambda: to run the application logic
- Amazon API Gateway: to expose the API endpoint to register and unregister users
- Amazon SNS: to send notifications to registered users

The application uses the Twitter APIs to monitor the specified Twitter user's followers and sends notifications to registered users when there is a change in the user's follower count. Users can register and unregister themselves from the notification service by calling the API endpoint exposed by the Amazon API Gateway.

## AWS SAM Pipeline

The application is deployed using the AWS SAM pipeline, which is an extension of the AWS CodePipeline service. The pipeline automates the building, testing, and deployment of the application, ensuring that it is delivered with high quality and reliability. The AWS SAM pipeline follows the following steps:

1. **Source**: The pipeline starts with the source stage, which fetches the application code from the Git repository.
2. **Build**: In the build stage, the pipeline builds the application package using the AWS SAM CLI and tests the package to ensure it meets the quality standards.
3. **Deploy**: In the deploy stage, the pipeline deploys the application package to AWS CloudFormation, which creates the necessary resources in the AWS account.
4. **Test**: In the test stage, the pipeline executes automated tests to ensure that the deployed application works as expected.
5. **Review**: In the review stage, the pipeline generates a review environment for manual testing and review.
6. **Approve**: After the review stage, the pipeline waits for approval to promote the application to production.
7. **Deploy to Production**: In the final stage, the pipeline deploys the application to production.

The AWS SAM pipeline ensures that the application is delivered with high quality, reliability, and scalability, following best practices for continuous delivery.

## Conclusion

The Serverless Twitter Follower Notification Application demonstrates how AWS SAM can be used to build and deploy serverless applications efficiently. By leveraging AWS Lambda, API Gateway, and SNS services, the application provides a scalable and efficient solution for monitoring Twitter followers. The AWS SAM pipeline ensures that the application is delivered with high quality and reliability, following best practices for continuous delivery.
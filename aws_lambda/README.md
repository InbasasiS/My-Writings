# AWS Lambda - Server Less Computing

## Why lambda

There are cases where we want our application not to run 24/7 (it is wasteful to have a web server like apache or nginx running 24/7 waiting for that event to occur and then perform an action in response to it) or there are cases 1only periodic tasks to be performed or incase of using certain background jobs in our application will block threads for long time for eg. Huge file processing tasks from ftp server, periodic API calls etc.

In these cases, AWS Lambda can be a simple and more effective,

## What is lambda functions

Lambda is a AWS solution for function as a service(FAAS), where we can code and trigger backgound tasks as separate functions(lambda) without worrying about server maintenance which means AWS will manage all the memory, CPU, network, and other resources.

It can scale up and down based on the traffic. When there’s a lot of requests the function automatically scales to accommodate the growing needs. Similarly, when the need dies down, the service scales down as well, to conserve resources.

The server will not run for all 24/7, it will be waiting for a event to take place, Whenever a lambda is triggered, the configured code will be deployed and then excuted so it will ideal all other time, that means its serverless, stateless and reduces the wastage of resources.

## Some Events to trigger lambda function: 
Lambda function can be whenever a file uploaded in amazon s3(data storage) or any ftp server or through amazon API gateway, any transaction on Dynamo DB or using any other aws services like Amazon SES(mail service), SNS, SQS etc.

## Usefull Reads
[aws-lambda-use-cases](https://www.simform.com/serverless-examples-aws-lambda-use-cases/)

[aws-lambda-examples](https://www.simform.com/serverless-aws-lambda-examples/)

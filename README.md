# MoviePosterDesign-using-AWS-Bedrock

**UseCase: Media and Entertainment UseCase**

Generate Movie Poster design using AWS Bedrock. In AWS Bedrock we are having many different Foundation models like Amazon Titan, LLama, Stability etc. Here in this use case as we have to generate the image so we are using **Stability** foundation model in** AWS Bedrock**.


**Architecture:** 

A prompt is sent through API Gateway that is a REST API then this prompt acts as an event to the lambda function , then the lambda function triggers where the promopt and inference parameters are sent to the AWS Bedrock as already mentioned the Stability model is invoke in the function then the AWS Bedrock uses the Stability model to generate the image acording to the prompt user provided. After generating the image it is stored in S3 bucket with the uodated date and time. In which we can access the image by using the Signed URL link which is again sent to the user for acccessing the image.

So here is the complete architecture for generating the Movie Poster Design using AWS Bedrock, API Gateway, S3 and Lambda services.

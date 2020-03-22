# AWS [Lambda](https://github.com/awsdocs/aws-lambda-developer-guide/tree/master/doc_source)
> Run code without thinking about servers. Pay only for the compute time you consume
* It’s a compute service that lets you run code without provisioning or managing servers.
* It executes your code only when needed and scales automatically, from a new requests per day to thousands per second.
* You pay only for the compute time you consume - there’s no charge when your code is not running.
* With this, you run functions o process events.

### Functions
* It's a resource that you can invoke to run your code in AWS Lambda.
* A function has a code that processes events, and a runtime that passes requests and responses between Lambda and the function code.

### Runtime
* Lambda runtimes allow functions in different languages to run in the same base execution environment
* You configure your function to use a runtime that matches your programming language.
* The runtime sits in between the Lambda service and your function code, relaying invocation events, context information, and responses between the two.

### Event
* It’s a JSON formatted document that contains data for a function to process.
* The Lambda runtime converts the event to an object and passes it to your function code.

### Modes
* **Sync:** When you invoke a function synchronously, Lambda runs the function and waits for a response. When the function execution ends, Lambda returns the response from the function's code with additional data, such as the version of the function that was executed. 
* **Async:** When you invoke a function asynchronously, you don't wait for a response from the function code. You hand off the event to Lambda and Lambda handles the rest.

## Serverless
It relates mainly to the FaaS architecture on AWS Lambda, Azure or Google cloud.

### Serverless with AWS Lambda
Serverless architecture lets function run as a service on AWS instead of running a full server.

### FaaS
Lambda, Google Cloud Functions, Azure Functions, etc.

* **1. Function as a service:** Is being able to deploy functions in the cloud, and then run those functions based on some type of event.
* **2. Difference between FaaS and Traditional Service:** where Traditional Service is a long lived server, that’s on some port that’s always on, that is probably listening some HTTP request to come in, that’s the difference. FaaS, they don’t do that. They’re not long-lived. They only spin up when they’re subscribing to an event and that events happens. And then, they shut down. They are stateless, that’s a big difference.
* **3. Serverless framework** which is different from a **Serverless architecture** (i.e. FaaS architecture on Lambda).

## What is Serverless?
Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

**Important to Note** that Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls (Functions as a Service).

some of the currently available cloud services:
1. AWS Lambda

2. Google Cloud Functions

3. Azure Functions

4. IBM OpenWhisk

5. Alibaba Function Compute

6. Iron Functions

7. Auth0 Webtask

8. Oracle Fn Project

9. Kubeless

## The diffrernce between Traditional & Serverless Architecture:
1. Pricing: The cost model of Serverless is execution-based: you’re charged for the number of executions. You’re allotted a certain number of seconds of use that varies with the amount of memory you require.

2. Networking: Serverless functions are accessed only as private APIs. To access these you must set up an API Gateway. This doesn’t have an impact on your pricing or process, but it means you cannot directly access them through the usual IP.

3. Environments: Serverless is as easy as setting up a single environment. Given that it’s pay per execution, this is a large improvement over traditional servers, you no longer need to set up dev, staging, and production machines.

4. Timeout: Too complex or long-running functions aren’t good for Serverless, but having a hard timeout makes it impossible to perform certain tasks. A hard limit on this time makes Serverless unusable for applications that have variable execution times, and for certain services which require information from an external source.

5. Scale: Scaling process for Serverless is automatic and seamless, but there is a lack of control or entire absence of control.

6. Functions as a Service (FaaS): is an implementation of Serverless architectures where engineers can deploy an individual function or a piece of business logic.

7. Stateless: With Serverless, everything is stateless, you can’t save a file to disk on one execution of your function and expect it to be there at the next.

## Kool-Aid For Amplify AWS:
is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications, powered by AWS.

AWS also provides us some features such as: 
1. Configure app backends and connect your app.
2. Deploy static web apps.
3. You can easily manage app content outside the AWS console.

4. Authentication.

5. DataStore.

6. Manage Users.

7. API (GraphQL, REST).

8. Interactions.

## GraphQL:
It provides a simple to use abstraction that helps you quickly create backends for your web and mobile applications on AWS. It is also used to **define application’s data model**.






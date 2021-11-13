# Cognito:
provides authentication, authorization, and user management for your web and mobile apps. Your users can sign in directly with a user name and password, or through a third party such as Facebook, Amazon, Google or Apple.

The two main components of Amazon Cognito:
1. User pools: 
is a user directory in Amazon Cognito. With a user pool, your users can sign in to your web or mobile app through Amazon Cognito, or federate through a third-party identity provider (IdP). Whether your users sign in directly or through a third party, all members of the user pool have a directory profile that you can access through an SDK. 
2. Identity pools: 
users can obtain temporary AWS credentials to access AWS services, such as Amazon S3 and DynamoDB. 

**Important to note that Amazon Cognito User pool and Udentity pool are used together**.

The **Goal** of using Cognito is to **setup and configure your application with Amplify Auth and go through a simple api to check the current auth session**.

How to configure Auth in our app:
1. By using this command: **amplify add auth**.

It will ask you these questions:
**? Do you want to use the default authentication and security configuration?**
    `Default configuration`
**? How do you want users to be able to sign in?**
    `Username`
**? Do you want to configure advanced settings?**
    `No, I am done.`


2. After doing the first command we are going to do **amplify push** To push changes to the cloud.

3. Then we need to install Amplify Libraries: implementation 'com.amplifyframework:aws-auth-cognito:1.28.3'
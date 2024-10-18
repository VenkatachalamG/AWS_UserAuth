# AWS_UserAuth

<h1>User Authentication with AWS Cognito</h1>

<p>This project implements user registration and login functionality using AWS Cognito in a serverless environment with AWS Lambda. It provides a RESTful API for managing user authentication, including password-based login and registration.</p>

<h2>Features</h2>
<ul>
    <li>User registration with email and password</li>
    <li>User login with email and password</li>
    <li>Secure user authentication through AWS Cognito</li>
    <li>IAM role permissions for Lambda function</li>
    <li>Easy integration with other AWS services</li>
</ul>

<h2>Technologies Used</h2>
<ul>
    <li>AWS Lambda (Node.js)</li>
    <li>AWS Cognito</li>
    <li>AWS SDK</li>
    <li>AWS IAM</li>
</ul>

<h2>Setup Instructions</h2>

<h3>Prerequisites</h3>
<ul>
    <li>An AWS account</li>
    <li>AWS CLI installed and configured</li>
    <li>Node.js installed</li>
</ul>

<h3>AWS Cognito Setup</h3>

<h4>Create a User Pool:</h4>
<ol>
    <li>Go to the AWS Cognito console and create a new user pool.</li>
    <li>Enable email-based sign-in and set up required attributes.</li>
</ol>

<h4>Create an App Client:</h4>
<ol>
    <li>Under the App clients section of your user pool, create a new app client.</li>
    <li>Make sure to enable <strong>ALLOW_USER_PASSWORD_AUTH</strong> in the authentication flows.</li>
</ol>

<h4>Update IAM Roles:</h4>
<ol>
    <li>Create a new IAM role for the Lambda function.</li>
    <li>Attach the <strong>AWSLambdaBasicExecutionRole</strong> and a policy allowing access to your Cognito user pool.</li>
</ol>

<h3>Testing :</h3>

![User Registration Authentication](https://github.com/user-attachments/assets/682710b7-6327-4802-bbe1-5bde32af7455)
<strong><p>Test for User Registration</p></strong>

![User Login Authentication](https://github.com/user-attachments/assets/63efa660-1102-42b7-9354-b8626bed487c)
<strong><p>Test for User Registration</p></strong>

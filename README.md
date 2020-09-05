# serverless-npm-hello-world

using npm to install serverless

```
npm install -g serverless
```

Create service in current working directory

```
serverless create --template aws-nodejs
```

serverless service endpoint for local

```
npm install serverless-offline --save-dev
```

run in the local

```
serverless offline
```

deploying lambda function

```
$ serverless deploy
Serverless: Packaging service...
Serverless: Excluding development dependencies...
Serverless: Creating Stack...
Serverless: Checking Stack create progress...
........
Serverless: Stack create finished...
Serverless: Uploading CloudFormation file to S3...
Serverless: Uploading artifacts...
Serverless: Uploading service serverless-npm-hello-world.zip file to S3 (28.61 MB)...
Serverless: Validating template...
Serverless: Updating Stack...
Serverless: Checking Stack update progress...
..............................
Serverless: Stack update finished...
Service Information
service: serverless-npm-hello-world
stage: dev
region: us-east-1
stack: serverless-npm-hello-world-dev
resources: 11
api keys:
  None
endpoints:
  GET - https://e0okwuo8z2.execute-api.us-east-1.amazonaws.com/dev/hello
functions:
  hello: serverless-npm-hello-world-dev-hello
layers:
  None

*************************************************************************************************************************
Serverless: Announcing Metrics, CI/CD, Secrets and more built into Serverless Framework. Run "serverless login" to activate for free..
*************************************************************************************************************************

```

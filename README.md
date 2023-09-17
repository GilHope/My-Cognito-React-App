# Project Guide

Deploy infrastructure (Cognito User Pool, CloudFront Distribution, S3 Bucket) :

``` sam deploy --guided```

Then grab your User Pool id and User Pool Client Id and modify the file awsexports.js with these values

Then you can start the app in local mode:

```npm run start```

Build the app to generate your static website

```npm run build```

Sync the static website to your s3 bucket

```aws s3 sync build s3://your-s3-bucket-name```

[For a video guided tutorial, checkout Majestic.cloud on YouTube](https://www.youtube.com/watch?v=WymSgBVrD9s&t=345s)


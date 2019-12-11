    What is the URL to your forked git repo of the project? https://github.com/dgreeninger/aws_cfn_cust_res_mgr_demo
    What is the URL to your web hosted static S3 bucket? https://display-api-dev-dgreeninger-static-site.s3-us-west-2.amazonaws.com/index.html
    What is your web hosted static s3 bucket policy?

      {
        "Version": "2008-10-17",
          "Statement": [
            {
              "Sid": "PublicReadGetObject",
              "Effect": "Allow",
              "Principal": "*",
              "Action": "s3:GetObject",
              "Resource": "arn:aws:s3:::display-api-dev-dgreeninger-static-site/*"
            }
          ]
      }

    What is the github URL to the serverless framework plugin that was used to upload the static s3 content? https://github.com/k1LoW/serverless-s3-sync
    What is the name of the lambda function launched for managing the custom cloudformation resources? cfn-res-mgr-demo-lookup
    What is the name of the table that the state of the resources are stored in? cfn-res-mgr-dev-state
    Which javascript library is used to draw the icons? Paperjs?
    Which headers need to be present from the API server to allow for CORS? Access-Control-Allow-Origin and Access-Control-Allow-Credentials.
    What common ID type is used for the physical resource ID? the ID from the DDB table?
    Do custom resource lambda functions require IAM permissions to interact with cloudformation (not including the IAM managed role permission in AWSLambdaBasicExecutionRole)? apparently not?

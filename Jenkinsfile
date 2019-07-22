pipeline{agent any 
  stages{ stage('Clone Repo') 
          { steps 
                  { sh "export AWS_DEFAULT_REGION=us-east-1"
                    sh "aws cloudformation create-stack --stack-name Group41stack --template-body file://s3cft.json --region 'us-east-1'"}
           }
         }
      }


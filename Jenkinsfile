pipeline{agent any 
         stages{ stage('Clone Repo') 
          { steps 
                  { sh "export AWS_DEFAULT_REGION=us-east-1"
                   sh "aws cloudformation create-stack --stack-name ${stackname} --template-body file://s3cft.json --parameters ParameterKey=${buck_name} ,ParameterValue=${buck_value} --region 'us-east-1'"}
           }
         }
        }


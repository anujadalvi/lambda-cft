pipeline{
	agent any
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name ${Stack_Name} --template-body file://lambda_cft.json --parameters ParameterKey='functionname',ParameterValue='${params.Function_Name}' --region 'us-east-1'"
			}
	}
		
	
	}
}

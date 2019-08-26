pipeline {
	agent any
	stages {
		stage('Clone Repo') {
			steps {
				sh "export AWS_DEFAULT_REGION=us-east-1"
				sh "aws cloudformation create-stack --stack-name vk-test-jenkins-stack --template-body file://S3Bucket.json --region us-east-1"
			}
		}
	}
}

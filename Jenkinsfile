pipeline {
    agent any

    stages {
        stage('CloudFormation Provision') {
            steps {

                sh "aws cloudformation create-stack --stack-name myteststacks --template-body file://parent-stack.yaml --region ap-south-1 --parameters ParameterKey=Environment,ParameterValue=${params.Environment}"
            }
        }
    }
}

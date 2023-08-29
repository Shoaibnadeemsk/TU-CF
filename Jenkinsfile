pipeline {
    agent any
    options { timestamps() }

    stages {
        stage('CloudFormation Provision') {
            steps {

                sh "aws cloudformation deploy --template-file parent-stack.yaml --stack-name nadeemstack --parameter-overrides Environment=dev --region=us-east-1"
            }
        }
    }
}

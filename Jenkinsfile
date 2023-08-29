pipeline {
    agent any

    stages {
        stage('CloudFormation Provision') {
            steps {

                sh "aws cloudformation deploy --template-file --stack-name nadeemstack --parameter-overrides Environment=prod"
            }
        }
    }
}

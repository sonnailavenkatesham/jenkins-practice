pipeline{
    agent {node { label 'agent'}}

    stages{
        stage('terraform init'){
            steps{
                echo "Testing on Webhook"
                sh '''
                ls -l
                pwd
                '''
            }
        }
        stage('terraform plan'){
            steps{
                echo "Hello terraform plan"
                sh '''
                '''
            }
        }
    }
    post{
        always{
            echo "this command will run always"
        }
        success{
            echo "process is success"
        }
        failure{
            echo "process failed"
        }
    }
}
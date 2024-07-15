pipeline{
    agent {node { label 'agent'}}

    stages{
        stage('terraform init'){
            steps{
                sh '''
                ls -l
                pwd
                '''
            }
        }
        stage('terraform plan'){
            steps{
                sh '''
                terraform plan
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
pipeline {
    agent {node { label 'agent'}}

    stages {
        stage('Build') {
            steps {
                sh '''
                ls -l
                pwd
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post{
        always{
            echo 'this session will run always irrespective of success or failure'
        }
        success{
            echo 'this session will run when the all stages are success'
        }
        failure{
            echo 'this session will run when the stage get Error/failure'
        }
    }
}
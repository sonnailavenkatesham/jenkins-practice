pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
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
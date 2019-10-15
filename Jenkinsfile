pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
                bat 'npm run build'
            }
        }
        stage('Test') {
            steps {
                bat 'npm run test' 
                junit '**/target/*.xml' 
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
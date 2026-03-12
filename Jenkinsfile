pipeline {
    agent any
    tools {
        nodejs 'node' 
    }
    stages {
        stage('Installation') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                bat 'npm test'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }
    }
}
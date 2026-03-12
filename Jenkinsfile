pipeline {
    agent any
    tools {
        nodejs 'node' // Le nom que tu as donné dans la config de Jenkins
    }
    stages {
        stage('Installation') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }
    }
}
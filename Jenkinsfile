pipeline {
    agent any

    tools {
        // 'node' doit être le nom que tu as donné dans Administrer Jenkins > Tools
        nodejs 'node'
    }

    stages {
        stage('Installation') {
            steps {
                echo 'Installation des dépendances...'
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Exécution des tests unitaires...'
                bat 'npm test'
            }
        }

        stage('Build') {
            steps {
                echo 'Construction de l\'application...'
                echo 'Build terminé avec succès.'
            }
        }
    }

    post {
        success {
            echo '--------------------------------------------------'
            echo 'Bravo, déploiement réussi !'
            echo '--------------------------------------------------'
        }
        failure {
            echo 'Le build a échoué. Vérifiez les erreurs dans la console.'
        }
    }
}
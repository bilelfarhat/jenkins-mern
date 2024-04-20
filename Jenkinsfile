pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Installez les dépendances Node.js
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                // Exécutez votre script de test
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}

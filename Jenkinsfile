pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    // Assurez-vous que Node.js est installé et utilisez la version appropriée
                    sh 'nvm use 8.17.0'
                    // Installez les dépendances Node.js
                    sh 'npm install'
                }
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

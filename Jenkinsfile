pipeline {
    agent any
    
    environment {
        PATH = "$PATH:../usr/bin"
    }
    
    stages {
        stage('Build') {
            steps {
                // Installez les dépendances Node.js
                sh 'npm install'
            }
        }
        // Autres étapes de votre pipeline...
    }
}

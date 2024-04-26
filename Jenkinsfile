pipeline {
    agent any
    tools {
        nodejs '14.21.3'
    }

    stages {
        stage('Build') {
            steps {
                // Installez les dépendances Node.js
                sh 'npm install'
            }
        }
        // Other stages of your pipeline...
    }
}
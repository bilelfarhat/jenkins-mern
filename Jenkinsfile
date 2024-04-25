pipeline {
    agent any
    
    stages {
        stage('Build') { 
            steps {
                script {
                    // Nettoyer les anciennes dépendances et vider le cache npm
                    sh 'rm -rf node_modules/*'
                    sh 'npm cache clean --force'
                    
                    // Installer les dépendances à partir du fichier package.json
                    sh 'npm install'
                }
            }
        }
    }
}

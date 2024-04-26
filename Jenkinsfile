pipeline {
    agent any
    tools {
        nodejs 'nodejs'
    }

    stages {
        stage('Build') {
            steps {
                // Installez les dépendances Node.js
                sh 'npm install'
            }
        }
         stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
         stage('Deliver') {
            steps {
                sh './jenkins/scripts/deliver.sh'
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                sh './jenkins/scripts/kill.sh'
            }
        }
        
    }
}

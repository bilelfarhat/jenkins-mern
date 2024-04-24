pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Install npm
                sh 'sudo apt-get update && sudo apt-get install -y npm'
                // Install dependencies
                sh 'npm install'
            }
        }
        // Other stages of your pipeline...
    }
}

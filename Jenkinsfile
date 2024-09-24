pipeline {
    agent any

    tools {
        nodejs 'NodeJS 14'  // This is the name you set in the NodeJS configuration
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add testing commands here if any
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add deployment steps here if any
            }
        }
    }
}

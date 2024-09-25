pipeline {
    agent any

    tools {
        nodejs 'NodeJS 14'  // The name you set in the NodeJS configuration
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
                echo 'Running tests...'
                sh 'npm test'
            }
        }
        stage('Lint') {
            steps {
                echo 'Linting the code...'
                sh 'npm run lint'
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

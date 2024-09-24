pipeline {
    agent any
    
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
                // Add your testing steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }
}

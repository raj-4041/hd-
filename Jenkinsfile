pipeline {
    agent any

    tools {
        nodejs 'NodeJS 14'  // Make sure this matches the NodeJS configuration in Jenkins
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'  // Installs all dependencies
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test'  // This will run tests if you've defined them in your package.json
            }
        }

        stage('Lint') {
            steps {
                echo 'Linting the code...'
                sh 'npm run lint'  // Make sure to add a lint script in your package.json for ESLint or other linters
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying with Docker...'
                sh 'docker build -t myapp .'  // Docker build step, change 'myapp' to your Docker image name
                sh 'docker run -d -p 8080:8080 myapp'  // Docker run step, make sure the port matches your app config
            }
        }
    }

    post {
        always {
            echo 'Sending notifications...'
            
        }
    }
}

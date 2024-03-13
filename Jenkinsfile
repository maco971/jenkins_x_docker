pipeline {
    agent any

    tools {
        // Use JDK and Maven defined in Jenkins Global Tool Configuration
        jdk 'JDK11'
        maven 'Maven3.9.6'
    }

    stages {
        stage('Build') {
            steps {
                // Building Docker image
                script {
                    docker.build('my-node-app')
                }
            }
        }
        stage('Test') {
            steps {
                // Add steps to test your application
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                // Add steps to deploy your application
                echo 'Deploying application...'
            }
        }
    }
}

pipeline {
  agent {
    label 'master'
  }
    tools {
        // Use JDK and Maven defined in Jenkins Global Tool Configuration
        jdk 'java2'
        maven 'mvn3.9.6'
        nodejs 'nvm14.21.3'
    }

    stages {
        stage('Build') {
            steps {
                sh '''
                  node --version
                  git --version
                  curl --version
                '''
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

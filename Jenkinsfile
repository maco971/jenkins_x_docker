pipeline {
    agent{
        docker{
            image "node:14.21.3"
            image "maven:3.9.6-amazoncorretto-21"
        }
        
        
    }
    
    tools {
        // Assurez-vous que ces outils sont configurés avec ces noms dans Jenkins
        jdk 'java2'
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/maco971/jenkins_x_docker.git'
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Skipping Test stage for now'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Skipping Deploy stage for now'
            }
        }
    }
}

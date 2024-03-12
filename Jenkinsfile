pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                script {
                    docker.build('node-app:v1')
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    docker.withRegistry('https://your-docker-registry.com', 'docker-credentials-id') {
                        docker.image('node-app:v1').push('latest')
                    }
                }
            }
        }
    }
}

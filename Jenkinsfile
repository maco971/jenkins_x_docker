pipeline {
    agent any
    
    tools {
        // Define the JDK tool named "Java11" using AdoptOpenJDK 11
        jdk 'java2'
        // Define the Maven tool named "Maven_3.9.6" using Maven 3.9.6
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                // Checkout the source code from your GitHub repository
                git 'https://github.com/your-username/your-repo.git'
                
                // Run Maven to build the project
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                // Run your tests here
            }
        }
        stage('Deploy') {
            steps {
                // Deploy your application
            }
        }
    }
}

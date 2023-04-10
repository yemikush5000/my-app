pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Clone your Git repository
                git url: 'https://github.com/yemikush5000/my-app.git'
            }
        }
        
        stage('Build') {
            steps {
                // Run Maven to build the project
                sh 'mvn clean install'
            }
        }
        
        stage('Test') {
            steps {
                // Run Maven to run unit tests
                sh 'mvn test'
            }
        }
    }
}

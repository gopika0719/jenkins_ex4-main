pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/gopika0719/jenkins_ex4-main.git'
            }
        }
        stage('Build') {
            steps {
                // Change "sh" to "bat" for Windows!
                bat 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                // Change "sh" to "bat" for Windows!
                bat 'mvn test'
            }
        }
    }
}
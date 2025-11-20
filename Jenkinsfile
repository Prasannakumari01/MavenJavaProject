pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Prasannakumari01/MavenJavaProject.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
            }
        }
    }
}


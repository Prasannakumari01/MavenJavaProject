pipeline {
    agent any

    tools {
        maven "MAVEN_HOME"
        jdk "JAVA_HOME"
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Prasannakumari01/MavenJavaProject.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }

    post {
        success {
            echo 'Build Successful!'
        }
        failure {
            echo 'Build Failed!'
        }
    }
}

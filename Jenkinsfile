pipeline {
    agent any
    tools {
        maven 'M3'   // Match Maven tool name in Jenkins
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Debug') {
            steps {
                bat 'echo JAVA_HOME=%JAVA_HOME%'
                bat 'echo MAVEN_HOME=%MAVEN_HOME%'
                bat 'mvn --version'  // Verify Maven is recognized
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}

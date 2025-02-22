pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm // Checks out code from GitHub
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package' // Builds the Maven project
            }
        }
    }
}

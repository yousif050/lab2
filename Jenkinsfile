pipeline {
    agent any
    tools {
        jdk 'JDK21'
        maven 'M3' // Name of the Maven tool configured in Jenkins
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                bat 'mvn clean package' // Use 'bat' for Windows
            }
        }
    }
}

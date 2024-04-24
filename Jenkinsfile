pipeline {
    agent any
    environment {
        PATH = "/usr/bin:$PATH" // Add Maven to the PATH
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install' // Use 'mvn' directly since it's now in the PATH
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test' // Use 'mvn' directly since it's now in the PATH
            }
        }
    }
}

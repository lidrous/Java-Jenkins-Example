pipeline {
    agent any
    environment {
        PATH+EXTRA = '/usr/bin/mvn/bin' // Append Maven to the existing PATH
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





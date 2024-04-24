pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '/usr/bin/mvn clean install'
            }
        }
        stage('Test') {
            steps {
                sh '/usr/bin/mvn test'
            }
        }
    }
}


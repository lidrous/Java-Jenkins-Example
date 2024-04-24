pipeline {
    agent any
    
    environment {
        MAVEN_HOME = tool 'Maven'
    }
    
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/your_username/your_repository.git'
                sh '${MAVEN_HOME}/bin/mvn compile'
            }
        }
        stage('Run') {
            steps {
                sh 'java -cp target/classes Main'
            }
        }
    }
}









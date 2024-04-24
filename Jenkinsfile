pipeline {
    agent any
    
    environment {
        MAVEN_HOME = tool 'Maven'
    }
    
    stages {
        stage('Build') {
            steps {
                git url: 'https://github.com/lidrous/Java-Jenkins-Example.git'
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










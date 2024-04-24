pipeline {
    agent any
    
    environment {
        MAVEN_HOME = tool 'Maven'
    }
    
    stages {
        stage('Build') {
            steps {
                sh '${MAVEN_HOME}/bin/mvn clean install'
            }
        }
    }
}








pipeline {
    agent any 
    stages {
        stage('----Clean----') { 
            steps {
                sh "rm -rf pipeline-app"
                sh "mvn clean"
            }
        }
        stage('----Test----') { 
            steps {
                sh "mvn test"
            }
        }
        stage('----Deploy----') { 
            steps {
                sh "mvn package"
            }
        }
    }
}

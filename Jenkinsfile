pipeline {
    agent any 
    stages {
        stage('----Clean----') { 
            steps {
                sh "mvn clean"
            }
        }
        stage('----Test----') { 
            steps {
                sh "mv test"
            }
        }
        stage('----Deploy----') { 
            steps {
                sh "mvn deploy"
            }
        }
    }
}

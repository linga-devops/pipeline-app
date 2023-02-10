pipeline {
    agent any 
    stages {
        stage('----Clean----') { 
            steps {
                sh "rm -rf pipeline-app"
                sh "mvn clean"
                echo "This is triggered form clean stage"
            }
        }
        stage('----Test----') { 
            steps {
                sh "mvn test"
                echo "This is triggered form test stage"
            }
        }
        stage('----Deploy----') { 
            steps {
                sh "mvn package"
                echo "This is triggered form package stage"
            }
        }
    }
}

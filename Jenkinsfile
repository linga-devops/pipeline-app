pipeline {
    agent any 
    stages {
        stage('----Clean----') { 
            steps {
                sh "rm -rf pipeline-app"
                sh "git clone https://github.com/linga-devops/pipeline-app.git"
                sh "mvn clean -f pipeline-app"
                echo "This is triggered form clean stage"
                echo "===================================="
            }
        }
        stage('----Test----') { 
            steps {
                sh "mvn test -f pipeline-app"
                echo "This is triggered form test stage"
                echo "=========================================="
            }
        }
        stage('----Deploy----') { 
            steps {
                sh "mvn package -f pipeline-app"
                echo "This is triggered form package stage"
                echo "===================================="
            }
        }
    }
}

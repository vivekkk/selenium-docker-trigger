//Jenkinsfile (Declarative Pipeline)

pipeline {
    // master executor should be set to 0
    agent any
    stages {
        stage('Initialize the docker compose') {
            steps {
                //sh
                bat "docker compose up -d hub chrome firefox"
            }
        }
        stage('Build Image') {
            steps {
                //sh
                bat "docker compose up testng"
            }
        }
        
    }
}

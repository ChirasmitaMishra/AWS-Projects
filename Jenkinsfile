pipeline {
    agent { label 'agent1' }
    stages {
        stage('Code Checkout...'){
            steps{
                git branch: 'main', url: 'https://github.com/ChirasmitaMishra/AWS-Projects.git'
            }
        }
        stage('Build') { // First stage: Build
            steps {
                echo 'Building Container...'
                // Commands to build the project
                //sh 'docker-compose up -d' 
                  sh 'docker-compose -f /web-app-with-db/src/docker-compose.yml up'
                //sh 'sudo docker run --name nginx-jenkins -d nginx'
            }
        }
        
        }
    }

pipeline {
    agent any
 
    tools {
        maven 'maven3'
    }
 
    stages {
        stage('Install') {
            steps {
				sh "whoami"
                sh "mvn clean install"
            }
        }
		
		stage('Build Docker image') {
            steps {
                sh "sudo docker build -t jonastavares/spring-petclinic:latest ."
            }
        }
		
		stage('Run Docker image') {
            steps {
                sh "sudo docker run -p 9000:8080 jonastavares/spring-petclinic:latest"
            }
        }
    }
}
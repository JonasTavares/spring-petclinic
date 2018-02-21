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
                sh "sudo docker build -t jonasjavares/spring-petclinic:latest ."
            }
        }
		
		stage('Run Docker image') {
            steps {
                sh "sudo docker run -it 9000:9000 jonastavares/spring-petclinic:latest ."
            }
        }
    }
}
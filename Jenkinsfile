pipeline {
	agent none
    tools {
        maven 'maven3'
    }
	
	stages{
		stage('Checkout'){
			steps{
				checkout scm
			}
		}
		
		stage('Build application'){
			steps{
				sh 'mvn -version'
			}
		}
	}

 
}
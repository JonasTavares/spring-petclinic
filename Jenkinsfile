pipeline {

    tools {
        maven 'maven3'
    }
	def app
	
	stages{
		stage('Checkout'){
			checkout scm
		}
		
		stage('Build application'){
			sh 'mvn -version'

		}
	}

 
}
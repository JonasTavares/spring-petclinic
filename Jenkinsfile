node {

	def app
	
	stage('Checkout'){
		checkout scm
	}
	
	stage('Build application'){
		steps{
			sh 'mvn clean install'
		}
	}

 
}
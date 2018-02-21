node {

	def app
	
	stage('Checkout'){
		checkout scm
	}
	
	stage('Build application'){

		sh 'mvn clean install'

	}

 
}
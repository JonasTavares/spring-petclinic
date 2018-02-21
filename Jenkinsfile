node {

	def app
	
	stage('Checkout'){
		checkout scm
	}
	
	stage('Build application'){
		withMaven(maven: 'Oracle BPM Quickstart 12.2.1'){
		
			sh 'mvn clean install'
		}

	}

 
}
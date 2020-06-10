pipeline{
	agent any
	
	environment{
		PATH = "/home/dz-jp-11/Desktop/apache-maven-3.6.0-bin/apache-maven-3.6.0"
	}
	
	stages {
		stage("Maven Build") {
			steps {
				sh 'mvn clean install'
			}
		}
	}
}


	

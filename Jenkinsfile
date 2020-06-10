pipeline{
	agent any
	
	environment{
		PATH = "/home/dz-jp-11/Desktop/apache-maven-3.6.0-bin/apache-maven-3.6.0"
	}
	
	stages {
		stage('Compile stage') {
			steps {
				sh 'mvn clean compile'	
			}
		}

		stage('Testing stage') {
			steps {
					sh 'mvn test'
			}
		}

		stage('Deployment stage') {
			steps {
				sh 'mvn deploy'
			}
		}
	}
}


	

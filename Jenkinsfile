pipeline{
	agent any
	
	environment{
		PATH = "/home/dz-jp-11/Desktop/apache-maven-3.6.0-bin/apache-maven-3.6.0"
	}
	stages {
		stage("git checkout") {
			steps {
				git url:'https://github.com/shubhamsainiksg7/spring-boot-hello-.git'
			}
		}
	
		stage("Maven Build") {
			steps {
				sh 'mvn clean install'
			}
		}
	}
}


	

pipeline{
	agent any
	
	environment{
		PATH = "/home/dz-jp-11/Desktop/apache-maven-3.6.0-bin:$PATH"
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
		stage("deploye") {
			steps {
				sh 'cp /var/lib/jenkins/workspace/pipeline-jenkins-example /home/dz-jp-11/Documents/Tomcat/apache-tomcat-8.5.20/webapps/pipeline-jenkins-example'
			}
		}
	}
}


	

pipeline{
	agent any

	stages {
		stage('Compile stage') {
			steps {
				withMaven(Maven : 'maven_3_6_0') {
					sh 'mvn clean compile'
				}
			}
		}

		stage('Testing stage') {
			steps {
				withMaven(Maven : 'maven_3_6_0') {
					sh 'mvn test'
				}
			}
		}

		stage('Deployment stage') {
			steps {
				withMaven(Maven : 'maven_3_6_0') {
					sh 'mvn deploy'
				}
			}
		}
	}
}


	

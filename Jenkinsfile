pipeline{
	agent any

	stages {
		stage('Compile stage') {
			steps {
				withMaven(maven : 'maven_3_6_0') {
					sh 'mvn clean compile'
				}
			}
		}

		stage('Testing stage') {
			steps {
				withMaven(maven : 'maven_3_6_0') {
					sh 'mvn test'
				}
			}
		}

		stage('Deployment stage') {
			steps {
				withMaven(maven : 'maven_3_6_0') {
					sh 'mvn deploy'
				}
			}
		}
	}
}


	

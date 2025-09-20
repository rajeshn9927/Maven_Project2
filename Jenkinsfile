pipeline{
	agent any
	stages{
		stage("cleaning"){
			steps{
				sh 'mvn clean'
			}
		}
		stage("New Build"){
			steps{
				sh 'mvn install'
			}
		}
		stage("jar execution"){
			steps{
				sh 'java -jar target/MavenProject-v1.0.1.2.jar'
			}
		}
	}
}

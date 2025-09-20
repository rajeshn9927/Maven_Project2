pipeline{
	agent any
	stages{
		stage("cleaning"){
			steps{
				bat 'mvn clean'
			}
		}
		stage("New Build"){
			steps{
				bat 'mvn install'
			}
		}
		stage("jar execution"){
			steps{
				bat 'java -jar target/MavenProject-v1.0.1.2.jar'
			}
		}
	}
}

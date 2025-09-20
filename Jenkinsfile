pipeline{
	agent any
	stages{
		stage("cleaning"){
			steps{
				mvn clean
			}
		}
		stage("New Build"){
			steps{
				mvn install
			}
		}
		stage("jar execution"){
			steps{
				java -jar target/MavenProject-v1.0.1.2.jar
			}
		}
	}
}

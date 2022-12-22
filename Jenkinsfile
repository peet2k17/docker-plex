pipeline {
	agent any

	environment {
		dockerHome = tool 'JenkinsDocker'
		PATH = "$dockerHome/bin:$PATH"
	}

   stages{
		stage('Build Docker Image') {
			steps{
				script{
					dockerImage = docker.build("peet2k17/plex")
				}
			}
		}
   }
}
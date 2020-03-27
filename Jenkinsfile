pipeline {
    agent any

    stages {
		environment {
			PATH = "C:\\Program Files\\Git\\usr\\bin;C:\\Program Files\\Git\\bin;${env.PATH}"
			stage('Build') {
				steps {
					bat "mvn.cmd clean package"
					archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
				}
			}
		}
    }
}
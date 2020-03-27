pipeline {
    agent any
	
	environment {
		PATH = "C:\\Program Files\\Git\\usr\\bin;C:\\Program Files\\Git\\bin;${env.PATH}"
	}
	
	stages {
		stage('Build') {
			steps {
				bat ".\\mvn.cmd clean package"
				archiveArtifacts artifacts: '**\\target\\*.jar', fingerprint: true 
			}
		}
	}
}
pipeline {
    agent any
	
	stages {
		stage('Build') {
			steps {
				bat "mvn.cmd clean package"
				archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
			}
		}
	}
}
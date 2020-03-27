pipeline {
    agent any
	
	stages {
		stage('Build') {
			steps {
				bat "%M2_HOME%\\mvn.cmd clean package"
				archiveArtifacts artifacts: '**\\target\\*.jar', fingerprint: true 
			}
		}
	}
}
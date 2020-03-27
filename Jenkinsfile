pipeline {
    agent any

	def shell(command) {
		return bat(returnStdout: true, script: "sh -x -c \"${command}\"").trim()
	}

    stages {
        stage('Build') {
            steps {
				sh 'mvn.cmd clean package'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
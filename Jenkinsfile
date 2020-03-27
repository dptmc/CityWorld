pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
				sh 'mvn.cmd clean package'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
				bat 'mvn clean package'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
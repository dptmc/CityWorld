pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                if (isUnix())
				{
					sh "mvn clean package"
				}
                else
				{
					bat "mvn.cmd clean package"
				}
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
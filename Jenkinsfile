pipeline {
    agent { label 'linux' }
    stages {
        stage('SonarQube') {
            steps {
                script { scannerHome = tool 'SonarQube Scanner' }
                withSonarQubeEnv('SonarQube Scanner') {
                sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=test -Dsonar.analysis.mode="
            }
         }
        }
    }
}
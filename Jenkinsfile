pipeline {
    agent { label '!windows' }
    stages {
        stage('SonarQube') {
            steps {
                script { scannerHome = tool 'SonarScanner' }
                withSonarQubeEnv() {
                sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=test"
            }
         }
        }
    }
}
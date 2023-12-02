pipeline {
    agent { label '!windows' }
    stages {
         stage('terraform started') {
            steps {
                sh 'echo "Started...!" '
            }
        }
        stage('SonarQube') {
            steps {
                script { scannerHome = tool  name: 'SonarQube Scanner', type: 'hudson.plugins.sonar.SonarRunnerInstallation';}
                withSonarQubeEnv('SonarQube Scanner') {
                sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=test"
            }
         }
        }
    }
}
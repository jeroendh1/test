pipeline {
    agent { label '!windows' }
    stages {
         stage('terraform started') {
            steps {
                bat 'echo "Started...!" '
            }
        }
        // stage('SonarQube') {
        //     steps {
        //         script { scannerHome = tool 'SonarQube Scanner' }
        //         withSonarQubeEnv('SonarQube Scanner') {
        //         sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=test"
        //     }
        //  }
        // }
    }
}
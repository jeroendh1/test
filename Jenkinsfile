pipeline {
    agent { docker { image 'php:8.3.0-alpine3.18' } }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
            }
        }
    }
}
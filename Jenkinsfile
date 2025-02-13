pipeline {
    agent any
    stages {
        stage('NPM Install') {
            steps {
                bat 'npm install'
            }
        }
         stage('Run npm audit tests') {
            steps {
                bat 'npm run audit'
            }
        }
        stage('Run integration tests') {
            steps {
                bat 'npm run test'
            }
        }
    }
}
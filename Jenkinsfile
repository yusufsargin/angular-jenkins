pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
            stage('Test') {
                sh 'npm run test'
            }
            stage('Build'){
                sh 'npm build'
            }
        }
    }
}

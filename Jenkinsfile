pipeline {
    agent any
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
          }
        stage('Test') {
          steps{
            sh 'npm run test'
          }
        }
        stage('Build'){
          steps{
             sh 'npm build'
          }
        }
        stage('Serve App Local'){
          steps{
            sh 'npm run serve-app'
          }
        }
    }
}

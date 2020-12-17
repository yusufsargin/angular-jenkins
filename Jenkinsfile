pipeline {
    agent any
    stages {
        stage('Reflesh From Git'){
          steps{
            git 'pull origin master'
          }
        }
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
    }
}

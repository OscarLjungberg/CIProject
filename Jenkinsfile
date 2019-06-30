pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
         stage('dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
        stage('tests') {
            steps {
                sh 'npm run test'
            }
        }
        stage('deploy ') {
            steps {
                sh 'npm run deploy'
            }
        }
    }
}
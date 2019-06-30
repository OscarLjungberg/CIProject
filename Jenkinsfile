pipeline {
    agent any
    
    tools {nodejs "node"}

    // Camillas jenkinsfil
    stages {
        stage('Bygga') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build production files') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Testa') {
            steps {
                sh 'npm run test'
            }
        }
        stage('Deploya') {
            steps {
                sh 'run deploy'
            }
        }
    }
}

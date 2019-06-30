pipeline {
    agent  any
    tools {nodejs "node"}
       
    stages {
        stage('install dependencies') { 
            steps {
                sh 'npm install' 
            }
        }
            stage('Build production files') { 
            steps {
                sh 'npm run build'  
            }
        }
        stage('Test'){
            steps {
                sh 'npm run test'
            }
        }
        stage('Deploy'){
            steps {
                sh 'npm run deploy'
                echo 'Deploying.....'
        }
    }
}
}
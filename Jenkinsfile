pipeline {

    agent any
    
    stages{
    
        stage("build") {
    
            steps{
                sh 'docker compose build'
                sh 'docker compose up'
            }
        }
        stage("test") {
    
            steps{
                sh 'npm test'
                sh 'npm start'
            }
        }
    }
}
pipeline{
    agent any
    tools{
        nodejs 'nodejs'
    }
    stages{

        stage('Build'){
            steps{
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('scan'){
            steps{
                sh 'npm run sonar'
            }
        }
        /*stage('test'){
            steps{
                sh 'npm run test'
            }
        }*/
    }
}
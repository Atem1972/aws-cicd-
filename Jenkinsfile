pipeline {
    agent any
    stages{
        stage('git checkout') {
            steps{
                sh 'pwd'
            }
        }
        stage('ls command') {
            steps{
                sh 'ls'
            }
        }
        stage('build') {
            steps{
                sh 'echo show'
            }
        }
        stage('touch') {
            steps{
                sh 'touch gigi'
            }
        }
        stage('lamda') {
            steps{
                sh 'whoami'
            }
        }
        stage('git checkout') {
            steps{
                git branch: 'main', url: 'https://github.com/Atem1972/awscicd.git'
            }
        }


    }
}

pipeline {
    agent any
    stages{
        stage('pwd command') {
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
                sh 'echo build'
            }
        }
        stage('touch') {
            steps{
                sh 'touch gigi'
            }
        }
    }
}
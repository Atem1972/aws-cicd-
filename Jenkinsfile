pipeline {
    agent any


environment{    #declearing variable
  branch_NAME = 'main'
  GIT_URL = 'https://github.com/Atem1972/awscicd.git'
}








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
        stage('docker build') {
            steps{
                sh 'docke build -t awscicd .'
                sh 'docker images'
            }
        }
        stage('git checkout now') {   # THIS IS IMPORTANT IN A REPO THAT HAS MANY BRANCHES
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }


    }
}

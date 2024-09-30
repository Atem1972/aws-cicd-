pipeline {
    agent any


environment{    
  branch_NAME = 'main'
  GIT_URL = 'https://github.com/Atem1972/awscicd.git'
  IMAGE_TAG = 'atem1972/awscicd'
  IMAGE_VERSION = ${build_NUMBER}
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
                sh 'docker build -t "${IMAGE_TAG}":"${IMAGE_VERSION}" .'
                sh 'docker images'
            }
        }
        stage('git checkout now') {   
            steps{
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }


    }
}

pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/mdlockwood/jenkins', branch: 'master')
      }
    }
    stage('Test') {
      steps {
        echo 'hello'
      }
    }
    stage('Release') {
      steps {
        sleep 12
      }
    }
    stage('Deploy') {
      steps {
        sleep 10
      }
    }
    stage('Send_Reports') {
      steps {
        sleep 5
      }
    }
    stage('AWS') {
      steps {
        sh '''hostname
whoami
env'''
      }
    }
  }
}
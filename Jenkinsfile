pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/mdlockwood/jenkins', branch: 'master')
        sh '''env
whoami
hostname'''
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
        sh '''env
whoami
hostname'''
      }
    }
    stage('AWS') {
      steps {
        sh '''hostname
whoami
env'''
        node(label: 'aws-elastic-t2-micro') {
          sh '''echo "in a child step"
hostname
whoami
env'''
        }
        
        sh '''whoami
env
hostname'''
      }
    }
  }
}
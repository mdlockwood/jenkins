pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/mdlockwood/jenkins', branch: 'master')
      }
    }
  }
}
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello world!"'
      }
    }
    stage('Test') {
      environment {
        CI = 'true'
      }
      steps {
        sh './jenkins/scripts/test.sh'
      }
    }
  }
}
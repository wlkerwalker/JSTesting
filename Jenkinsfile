pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'yarn install'
      }
    }
    stage('test') {
      steps {
        sh 'yarn run test'
      }
    }
  }
}
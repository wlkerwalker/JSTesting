pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'yarn install && yarn run test'
      }
    }
  }
}
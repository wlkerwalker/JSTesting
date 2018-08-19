pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'yarn install'
      }
    }
    stage('sanity-check') {
      steps {
        input 'does this look ok to you?'
      }
    }
    stage('test') {
      steps {
        sh 'yarn run test'
      }
    }
  }
  post {
    always {
      deleteDir()
    }
  }
}
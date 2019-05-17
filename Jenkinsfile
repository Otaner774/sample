pipeline {
  agent any
  stages {
    stage('install') {
      steps {
        sh 'npm install'
      }
    }
    stage('build') {
      steps {
        sh 'npm run build'
      }
    }
    stage('test') {
      steps {
        sh 'npm test'
      }
    }
    stage('aprovee') {
      steps {
        input(message: 'Se aprueba???', submitter: 'otaner01')
      }
    }
  }
}
pipeline {
  agent any
  stages {
    stage('make') {
      agent any
      steps {
        sh 'make'
        sh './hello_exec'
      }
    }
  }
  triggers {
    pollSCM('*/1 * * * *')
  }
}
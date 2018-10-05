pipeline {
  agent any
  triggers { pollSCM('*/1 * * * *') }
  stages {
    stage('make') {
      agent any
      steps {
        sh 'make'
      }
    }
  }
}

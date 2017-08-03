pipeline {
  agent any
  stages {
    stage('Check') {
      steps {
        parallel(
          "Check": {
            sh 'printenv'
            
          },
          "Build": {
            sh 'ls -al'
            
          }
        )
      }
    }
    stage('Run') {
      steps {
        sh 'pwd'
      }
    }
  }
}
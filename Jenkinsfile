pipeline {
  agent any
  stages {
    stage('Git checkout') {
      steps {
        checkout scm
      }
    }

    stage('Application build') {
      steps {
        sh '''scripts/build.sh
'''
      }
    }

  }
}
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
        sh 'script scripts/build.sh'
      }
    }

  }
}

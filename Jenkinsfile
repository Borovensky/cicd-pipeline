pipeline {
  agent any
  stages {
    stage('Git checkout') {
      steps {
        script {
          stage('Checkout code') {
            steps {
              checkout scm
            }
          }
        }

      }
    }

  }
}
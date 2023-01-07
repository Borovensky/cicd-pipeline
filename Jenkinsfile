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

    stage('Tests') {
      steps {
        sh 'script scripts/test.sh'
      }
    }

    stage('Docker image Build') {
      steps {
        sh 'docker build -t cicd-pipeline'
      }
    }

  }
}
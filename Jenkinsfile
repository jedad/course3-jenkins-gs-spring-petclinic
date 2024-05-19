pipeline {
  agent any
  stages {
    stage('MVN Prep') {
      steps {
        echo 'Preparing...'
        sh './mvnw --version'
        sh '''pwd
ls'''
      }
    }

    stage('Build') {
      steps {
        echo 'Building...'
        sh './mvnw compile'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}
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
        sh '''ls --only-dirs
        tree jobs workspace'''
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}

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
        sh 'ls -al'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
        sh './mvnw test'
      }
    }

    stage('Package') {
      steps {
        echo 'Archiving...'
        sh './mvnw package'
      }
    }

    stage('Archive') {
      steps {
        archiveArtifacts 'pet-drop'
      }
    }

  }
}
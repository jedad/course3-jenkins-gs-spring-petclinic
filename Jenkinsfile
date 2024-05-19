pipeline {
  agent any
  stages {
    stage('Pipeline Test') {
      steps {
        sh '''
          echo "Start pipeline"
          pwd
          ls
            '''
      }
    }

    stage('MVN Test') {
      steps {
        sh './mvnw --version'
      }
    }

  }
}
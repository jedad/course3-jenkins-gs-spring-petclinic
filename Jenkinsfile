
pipeline {
    agent any
    stages {
        stage('Prep') {
            steps {
                echo 'Building...'
                sh './mvnw --version'
                // Add your build steps here
            }
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deploy steps here
            }
        }
    }
}

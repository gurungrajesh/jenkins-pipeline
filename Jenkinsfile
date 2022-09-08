pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "Hello World"'
          }
        }

        stage('test') {
          steps {
            echo 'Testing Phase'
          }
        }

      }
    }
    stage('staging') {
      step {
        echo "Building Staging"
      }
    }

  }
  environment {
    stage = 'build'
  }
}
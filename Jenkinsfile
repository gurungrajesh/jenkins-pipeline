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

  }
  environment {
    stage = 'build'
  }
}
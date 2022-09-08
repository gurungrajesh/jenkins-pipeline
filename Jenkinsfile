pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        input message: 'Do you want to continue', ok: 'Yes', parameters: [booleanParam('yes')]
      }
    }

  }
}
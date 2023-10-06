pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Hello World'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input 'Do we want to proceed?'
        echo 'Deployment'
      }
    }

  }
  environment {
    TEXT = 'Hello World'
  }
}
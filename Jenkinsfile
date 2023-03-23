pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'I want to develop'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'I want to Build'
          }
        }

        stage('Test') {
          steps {
            echo 'I want to Test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I want to deploy the Code'
          }
        }

      }
    }

  }
}
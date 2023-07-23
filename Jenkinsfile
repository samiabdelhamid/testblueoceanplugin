pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Starting Build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Starting Testing'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Starting Security Test'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying Done !!'
      }
    }

  }
}
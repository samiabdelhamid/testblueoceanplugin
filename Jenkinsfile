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
        input(message: 'Are you sure to deploy', ok: 'Yes, I am sure!')
        echo 'Deploying Done !!'
      }
    }

  }
}
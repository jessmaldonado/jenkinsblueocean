pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building'
          }
        }

        stage('Parallel Build') {
          steps {
            echo 'Building 2nd one...'
          }
        }

      }
    }

    stage('Testing') {
      steps {
        echo 'Testing'
      }
    }

    stage('Deploying') {
      steps {
        echo 'Deploying in Production'
      }
    }

  }
}
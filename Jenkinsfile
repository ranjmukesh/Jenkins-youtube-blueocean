pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test Step'
            echo 'test Parameter'
          }
        }

        stage('Test Parrallel') {
          steps {
            echo 'Test Parallel'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}
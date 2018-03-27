pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sleep 4
          }
        }
        stage('error') {
          steps {
            echo 'eaysway'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'test to deliver'
      }
    }
    stage('Deploy') {
      steps {
        echo 'good to go'
      }
    }
  }
}
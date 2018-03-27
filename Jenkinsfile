pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "how to build"'
          }
        }
        stage('') {
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
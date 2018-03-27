pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'call mvn package'
          }
        }
        stage('') {
          steps {
            bat(script: 'mvn package', returnStatus: true, returnStdout: true)
          }
        }
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'call mvn test'
          }
        }
        stage('') {
          steps {
            bat(script: 'mvn test', returnStatus: true, returnStdout: true)
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'good to go'
      }
    }
  }
}
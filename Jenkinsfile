pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'call mvn package'
        bat 'mvn clean'
      }
    }
    stage('Test') {
      steps {
        echo 'call mvn test'
      }
    }
    stage('Deploy') {
      steps {
        echo 'good to go'
      }
    }
  }
}
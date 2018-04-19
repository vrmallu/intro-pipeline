pipeline {
  agent any
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello World!'
            sh 'java -version'
          }
        }
        stage('Hello Venkat') {
          steps {
            sh 'java -version'
          }
        }
      }
    }
  }
}
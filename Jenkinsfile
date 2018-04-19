pipeline {
  agent {
    docker {
      image 'golang:1.10.1-alpine'
      label 'docker-cloud'
    }
    
  }
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            echo 'Hello ${MY_NAME}!'
            sh 'java -version'
          }
        }
        stage('Hello Venkat') {
          steps {
            sh 'go version'
          }
        }
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
  }
}
pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'sadgunreddy/image:latest' }
      }
      steps {
        sh 'sudo apt-get install nginx'
      }
    }
    stage('Front-end') {
      agent {
        docker { image 'node:16-alpine' }
      }
      steps {
        sh 'node --version'
      }
    }
  }
}

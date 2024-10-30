pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'sadgunreddy/image:latest' }
      }
      steps {
        sh 'nginx -V'
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

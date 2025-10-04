pipeline {
  agent any
  tools {
      nodejs 'node-24.9.0'
  }
  stages {
    stage('Build') {
      steps {
        sh 'node -v'
        sh 'npm install'
      }
    }
  }
}

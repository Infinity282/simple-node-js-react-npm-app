pipeline {
    agent any
    tools {
        nodejs 'node-24.9.0'
    }
    stages {
        stage('Prepare') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Deliver') { 
            steps {
                sh 'npm publish'
            }
        }
    }
}

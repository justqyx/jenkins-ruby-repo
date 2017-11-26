pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "Build"'
          }
        }
        stage('Build2') {
          steps {
            sh '''echo "Build2"
echo "Build2"
echo "Build2"
echo "Build2"
echo "Build2"
echo "Build2"'''
          }
        }
      }
    }
    stage('Test') {
      steps {
        sh 'echo "Test"'
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            sh 'echo "Deploy"'
          }
        }
        stage('Deploy2') {
          steps {
            sh 'echo "Deploy2"'
          }
        }
        stage('Deploy3') {
          steps {
            sh 'echo "Deploy3"'
          }
        }
      }
    }
  }
  environment {
    RAILS_ENV = 'test'
  }
}
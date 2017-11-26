pipeline {
  agent {
    docker {
      image 'ruby:2.2.5'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'echo "Build"'
      }
    }
    stage('Test') {
      steps {
        sh 'echo "Test"'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploy"'
      }
    }
  }
}
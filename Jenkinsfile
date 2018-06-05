pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('first stage') {
      steps {
        echo 'Hello $(MY_NAME)!'
      }
    }
    stage('Second stage') {
      steps {
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'MARY'
  }
}
pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('first stage') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Second stage') {
      steps {
        sh 'java -version'
      }
    }
  }
}
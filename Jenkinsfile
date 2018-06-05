pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('first stage') {
      steps {
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
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
    TEST_USER = credentials('test-user')
  }
}
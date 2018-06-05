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
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'MARY'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}
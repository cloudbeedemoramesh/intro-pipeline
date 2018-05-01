pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Say Hello') {
      options {
        timeout(time: 30, unit: 'SECONDS')
      }
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Continuing with deployment'
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'CloudBee'
  }
}
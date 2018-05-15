pipeline {
  agent none
  stages {
    stage('Beginning') { agent any
      steps {
        echo 'hello world'
        }
     }
    stage('Who am I?') { agent any
      steps {
        sh 'whoami'
        }
     }
  }
}

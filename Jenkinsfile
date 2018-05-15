pipeline {
  agent none
  environment {
    NODE_VER = '8.1.0'
  }
  stages {
    stage('Beginning') { agent any
      environment {
        NEW_VAR = 'foo'
      }
      steps {
        echo 'hello world'
        sh 'echo $NODE_VER'
        sh 'echo $(env.NEW_VAR)'
        }
     }
    stage('Who am I?') { agent any
      steps {
        echo "${env.NEW_VAR}"
        sh 'whoami'
        }
     }
  }
}

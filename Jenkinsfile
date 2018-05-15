pipeline {
  agent none
  environment {
    NODE_VER = '8.1.0'
    NEW_VAR = 'foo'
  }
  stages {
    stage('Beginning') { agent any
      steps {
        echo 'hello world'
        sh 'echo $NODE_VER'
        }
     }
    stage('Who am I?') { agent any
      steps {
        sh 'whoami'
        }
     }
    stage('Deploy to stage?') { agent none
      step {
        input 'Deploy to stage?' 
        }
     }
  }
}

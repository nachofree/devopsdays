pipeline {
  agent none
  environment {
    NODE_VER = '8.1.0'
    NEW_VAR = 'foo'
  }
  post {
    sh 'echo "we are done"'
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
      steps {
        input 'Deploy to stage?' 
        }
     }
  }
}

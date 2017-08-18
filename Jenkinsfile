pipeline {
  agent any
  stages {
    stage('print msg') {
      steps {
        parallel(
          "print msg": {
            echo 'hello'
            
          },
          "run a bash": {
            sh '''pwd
ls
whoami

sh ./hello.sh'''
            
          }
        )
      }
    }
  }
  environment {
    test = 't1'
  }
}
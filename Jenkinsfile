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
'''
            
          }
        )
      }
    }
  }
  environment {
    test = 't1'
  }
}
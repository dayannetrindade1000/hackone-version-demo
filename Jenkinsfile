pipeline {
  agent none
  stages {
    stage('Build') {
      agent any
      steps {
        bat 'echo comecando build - teste1...'
        sh 'python -m py_compile hello.py'
        stash(name: 'compiled-results', includes: '*.py*' )
      }
    }
  }
}

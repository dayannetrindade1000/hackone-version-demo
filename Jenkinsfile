pipeline {
  agent none
  stages {
    stage('Build') {
      agent any
      steps {
        bat 'echo comecando build - teste1...'
        bat 'python3.10.exe -m py_compile hello.py'
        stash(name: 'compiled-results', includes: '*.py*' )
      }
    }
  }
}

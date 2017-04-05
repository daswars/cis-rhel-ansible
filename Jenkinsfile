pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        parallel(
          "ansible show version": {
            sh 'ls -la'
            
          },
          "ls": {
            echo 'test123'
            
          },
          "sleep": {
            sleep 2
            
          }
        )
      }
    }
  }
}
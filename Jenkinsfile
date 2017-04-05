pipeline {
  agent none
  stages {
    stage('test') {
      steps {
        parallel(
          "ansible show version": {
            sh 'ls -la'
            
          },
          "ls": {
            echo 'test'
            
          },
          "sleep": {
            sleep 2
            
          }
        )
      }
    }
    stage('ende') {
      steps {
        echo 'end'
      }
    }
  }
}
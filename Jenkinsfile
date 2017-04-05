pipeline {
  agent none
  stages {
    stage('error') {
      steps {
        parallel(
          "error": {
            echo 'hello'
            
          },
          "foo": {
            echo 'foo2'
            
          }
        )
      }
    }
  }
}
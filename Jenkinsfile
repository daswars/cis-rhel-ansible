pipeline {
  agent {
    docker {
      image 'rndmh3ro/docker-centos7-ansible-latest'
    }
    
  }
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
  }
}
pipeline {
  agent {
    docker {
      image 'rndmh3ro/docker-centos7-ansible'
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
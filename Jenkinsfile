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
            sh 'ansible --version'
            
          },
          "ls": {
            sh 'ls -la'
            
          }
        )
      }
    }
  }
}
pipeline {
 
  agent {
    label 'docker_slave'
  }
 
  stages {

    stage('Tests_unitaires') {

      steps {
        sh 'composer install'
        sh 'composer test-all'
      }
    }
  }
}

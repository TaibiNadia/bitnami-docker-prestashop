pipeline {
 
  agent {
    label 'docker_agent'
  }
 
  stages {

    stage('Tests unitaires') {

      steps {
        sh 'composer install'
        sh 'composer test-all'
      }
    }
  }
}

pipeline {
 
  agent {
    label 'docker'
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

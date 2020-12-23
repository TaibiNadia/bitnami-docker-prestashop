pipeline {
 
  agent none
 
  stages {

      stage('Tests unitaires') {
       agent {
          label 'prestashop_agent'
      }
     
      steps {
        sh 'composer install'
        sh 'composer test-all'
      }
    }

      stage('build') {

      steps {
        sh 'docker-compose up -d --build'
     }

   }

  }
}

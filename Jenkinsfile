pipeline {
 
  agent {
    label 'prestashop_agent'
  }
 
  stages {

    stage('Tests unitaires') {

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

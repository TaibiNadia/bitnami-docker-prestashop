pipeline {
  agent {
      docker { image 'docker.io/bitnami/prestashop:1.7-debian-10' }
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

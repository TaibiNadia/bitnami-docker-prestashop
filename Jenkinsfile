pipeline {
  stages {

      stage('Tests unitaires') {
      agent { dockerfile true }
     
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

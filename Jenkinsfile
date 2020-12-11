pipeline {
 agent {
 label 'slave_docker'
 }
 stages {

 stage('Tests unitaires') {

 steps {
 sh 'composer test-all'
 }

 }
}

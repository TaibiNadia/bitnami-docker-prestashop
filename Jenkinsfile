pipeline {
 agent {
 label 'bitnami/prestashop'
 }
 stages {

 stage('Tests unitaires') {

 steps {
 sh 'composer test-all'
 }

 }
}

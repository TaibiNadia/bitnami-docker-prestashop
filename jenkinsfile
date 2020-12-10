pipeline {
 agent {
 label 'bitnami/prestashop'
 }
 stages {

 stage('Tests unitaires') {

 steps {
 sh 'mvn test'
 }

 }
}

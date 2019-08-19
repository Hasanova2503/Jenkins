pipeline {
   agent any
   stages {
       stage('Build') {
           steps {
              echo 'This is a minimal pipeline.'
              withMaven(maven : 'maven_3.5.3') {
                                    sh 'mvn clean compile'
                                }

           }
       }
       
       stage('Test') {
          steps {
              echo '2 + 2'
          }
       }
   }
}
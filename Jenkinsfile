pipeline {
   agent any
   stages {
       stage('Build') {
           steps {
              echo 'This is a minimal pipeline.'
           }
       }
       
       stage('Test') {
          steps {
              echo '2+2'
          }
       }
       
       stage('Compile Stage') {
          steps {
              withMaven(maven : 'maven_3.5.3') {
                                    bat 'mvn clean compile'
                                }

          }
       }
   }
}
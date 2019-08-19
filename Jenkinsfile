pipeline {
    agent any
    
    stages {
        stage('Example Build') {
           steps {
               withMaven(maven : '3.6.1') {
                                     sh 'mvn clean compile'
                                 }

           }
        }
        
        stage('Testing') {
           steps {
               withMaven(maven : '3.6.1') {
                                     sh 'mvn test'
                                 }

           }
        }
        
        stage('Deploy') {
           steps {
               withMaven(maven : '3.6.1') {
                                     sh 'mvn deploy'
                                 }

           }
        }
    }
}
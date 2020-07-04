pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "Hello World"'
                 sh '''
                     echo "Multiline shell steps works too"
                     ls -lah
                 '''
             }
         }
         stage('Lint Makefile') {
              steps {
                  sh 'make all'
              }
         }
         stage('') {
              steps {
                  withAWS(region:'us-west-2',credentials:'aws-static') {
                  
              }
         }
     }
}
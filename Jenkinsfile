pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
                     python3 -m venv ~/.devops 
            '''
        sh '''
             .  ~/.devops/bin/activate
           '''
      }
    }

    stage('Lint Makefile') {
      steps {
        sh 'make all'
      }
    }

  }
}
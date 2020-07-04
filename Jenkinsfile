pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
                     echo "Multiline shell steps works too"
                     ls -lah
                     python3 -m venv ~/.devops
	                 source  ~/.devops/bin/activate
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
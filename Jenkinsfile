pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'echo %Name%'
          }
        }

        stage('Build2') {
          steps {
            bat 'echo Build2'
          }
        }

      }
    }

    stage('Test') {
      steps {
        bat 'echo Test'
      }
    }

  }
  environment {
    Name = 'Firststage'
  }
}
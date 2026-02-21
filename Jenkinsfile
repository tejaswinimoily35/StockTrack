pipeline {
  agent any

  stages {

    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo 'Dummy build step – no actual build required'
      }
    }

    stage('Test') {
      steps {
        echo 'Dummy test step – no tests available'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Dummy deployment step completed'
      }
    }

  }
}

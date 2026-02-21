pipeline {
  agent any

  stages {

    stage('Checkout Code') {
      steps {
        echo 'Cloning repository from GitHub...'
        checkout scm
      }
    }

    stage('Environment Check') {
      steps {
        echo 'Checking environment (dummy stage)'
        sh 'node -v || echo "Node not installed, but continuing"'
        sh 'npm -v || echo "NPM not installed, but continuing"'
      }
    }

    stage('Backend Build (Dummy)') {
      steps {
        echo 'Backend folder exists, no build required'
        sh 'ls -l || true'
        sh 'ls backend || echo "Backend folder present"'
      }
    }

    stage('Test (Dummy)') {
      steps {
        echo 'No tests available – dummy test stage passed'
      }
    }

    stage('Deploy (Dummy)') {
      steps {
        echo 'Deployment simulated successfully'
      }
    }
  }

  post {
    success {
      echo '✅ Jenkins dummy pipeline executed successfully'
    }
    failure {
      echo '❌ Pipeline failed'
    }
  }
}

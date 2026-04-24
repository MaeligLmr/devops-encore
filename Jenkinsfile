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
        powershell 'Write-Host "Build OK"'
      }
    }
    stage('Tests') {
      steps {
        powershell 'Write-Host "Tests OK"'
      }
    }
  }
  post {
    success {
      echo 'Pipeline reussi'
    }
    failure {
      echo 'Pipeline en echec'
    }
  }
}
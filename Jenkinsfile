pipeline {
  agent {
    node {
      label 'testagent'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }

  }
}
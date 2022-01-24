pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'done'
          }
        }

        stage('wait 5') {
          steps {
            sleep 5
            echo 'waited 5 seconds'
          }
        }

      }
    }

    stage('error') {
      steps {
        echo 'pipeline build and ran'
      }
    }

  }
}
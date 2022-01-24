pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'testing SSH'
            sshagent(credentials: ['RemoteCredentials']) {
              sh 'ssh -tt-o StrictHostKeyChecking=no -l jenkins 10.20.68.29 -a'
            }

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

  }
}
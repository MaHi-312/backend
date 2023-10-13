pipeline {
    agent { label 'workstation'}

    options {
        ansiColor('xterm')
    }

    stages {

      stage('Download Dependencies'){
        steps {
           sh 'npm install'
        }
      }
      stage('code quality'){
        steps {
           sh 'npm install'
        }
      }

      stage('Unit tests'){
        steps {
           echo 'CI'
        }
      }

      stage('Release'){
        steps {
           echo 'CI'
        }
      }
    }
}

////
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
           sh 'sonar-scanner -Dsonar.host.url=http://172.31.20.139:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=backend -Dsonar.qualitygate.wait=true'
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
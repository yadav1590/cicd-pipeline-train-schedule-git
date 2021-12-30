pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''date
uptime
hostname'''
          }
        }

        stage('build') {
          steps {
            echo 'Hello World'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 15
      }
    }

  }
}
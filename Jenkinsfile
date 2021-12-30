pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''date
time
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
        node(label: 'linux')
      }
    }

  }
}
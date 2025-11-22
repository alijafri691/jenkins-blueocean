pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh '''pwd
ls'''
          }
        }

        stage('build par') {
          steps {
            echo 'build par'
          }
        }

      }
    }

    stage('Test') {
      steps {
        sh 'date'
      }
    }

    stage('Prod') {
      steps {
        echo 'Prod'
      }
    }

  }
}
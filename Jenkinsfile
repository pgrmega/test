pipeline {
  agent any
  stages {
    stage('First step') {
      parallel {
        stage('First step') {
          steps {
            echo 'hello'
          }
        }
        stage('Parallel Step') {
          steps {
            pwd()
            sh 'echo A�e'
          }
        }
      }
    }
    stage('Second step') {
      steps {
        sleep 4
      }
    }
  }
}
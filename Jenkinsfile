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
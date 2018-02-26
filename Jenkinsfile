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
            readFile 'test.txt'
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
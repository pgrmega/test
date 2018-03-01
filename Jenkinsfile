pipeline {
  agent any
  parameters {
    booleanParam(name: 'run stage1',
                defaultValue: true,
                description: 'activate stage1')
  }
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

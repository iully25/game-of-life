pipeline {
  agent any
  stages {
    stage('game of life') {
      steps {
        parallel(
          "game of life": {
            build(job: 'gameoflife', quietPeriod: 5, wait: true)
            
          },
          "test": {
            timestamps() {
              echo 'Hello'
            }
            
            
          }
        )
      }
    }
    stage('maven') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
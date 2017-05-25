pipeline {
  agent any
  stages {
    stage('start') {
      steps {
        build(job: 'gameoflife', quietPeriod: 5, wait: true)
      }
    }
  }
}
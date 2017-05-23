pipeline {
  agent any
  stages {
    stage('start') {
      steps {
        build(job: 'test', quietPeriod: 5, wait: true)
      }
    }
  }
  environment {
    some = 'value'
  }
}
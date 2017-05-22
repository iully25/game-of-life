pipeline {
  agent any
  stages {
    stage('start') {
      steps {
        build(job: '1', propagate: true, quietPeriod: 5, wait: true)
      }
    }
  }
  environment {
    some = 'value'
  }
}
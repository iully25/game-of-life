pipeline {
  agent any
  stages {
    stage('start') {
      steps {
        build(job: 'new', propagate: true, quietPeriod: 5, wait: true)
      }
    }
  }
  environment {
    some = 'value'
  }
}
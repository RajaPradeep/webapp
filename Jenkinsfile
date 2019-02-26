pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        build(job: 'compile', quietPeriod: -5)
      }
    stage('test') {
      steps {
        build(job: 'test', quietPeriod: -5)
      }
    }
  }
}

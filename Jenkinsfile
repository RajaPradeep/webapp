pipeline {
  agent any
  
  stages {
    stage('compile stage') {
      steps {
        withmaven(maven: 'mavenjenkins'){
          sh 'mvn clean compile'
        }  
      }
    } 
    
    stage('testing stage') {
      steps {
        withmaven(maven: 'mavenjenkins'){
          sh 'mvn test'
        }
    }
  
  }


}

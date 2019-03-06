pipeline {
  agent any
  
  stages {
    stage('github checkout') {
        git 'https://github.com/RajaPradeep/webapp.git'
    }
    stage('packing stage') {
      steps {
        withmaven(maven: 'maven_3.6'){
          sh 'mvn clean package'
        }  
    }
      
    
    
    
    
    } 
}

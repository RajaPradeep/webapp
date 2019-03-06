node{
    stage('SCM Checkout'){
        git url:''
    }
    stage('MVN Package'){
        def mvnHome = tool name: 'maven_3.6', type: 'maven'
        def mvnCMD = "${mvnHome}/bin/mvn"
        sh "${mvnCMD} clean package"
    }
    
}

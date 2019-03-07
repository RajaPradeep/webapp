node{
    stage('SCM Checkout'){
        git url:'https://github.com/RajaPradeep/webapp.git'
    }
    stage('MVN Package'){
        def mvnHome = tool name: 'maven_3.6', type: 'maven'
        def mvnCMD = "${mvnHome}/bin/mvn"
        sh "${mvnCMD} clean package"
    }
//    stage('ssh into local machine'){
//        def remScript = "./home/ec2-user/remote_exec.sh"
//        sh "ssh -o StrictHostKeyChecking=no -i  /myprivkeyec2dynamo.pem ec2-user@172.31.81.16 && ${remScript}" 
//    }
    stage('Deploy'){
          sh "./deploy_tomcat.sh"   
    }
}

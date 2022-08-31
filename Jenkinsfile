pipeline {
  agent any
   stages{
    stage("Maven Build"){
      steps{
        sh "mvn clean package"
      }
    }
    stage("Deploy To tomcat"){
      steps{
       echo "india"
      }
    }
     post {
       success {
         archiveArtifacts artifacts: 'target/*.war'
       }
    }  
}

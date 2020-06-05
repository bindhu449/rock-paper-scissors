pipeline{
   agent { label 'Test' }
   tools {
      maven 'maven'
      jdk 'JAVA_HOME'
   }
   stages {
    stage ('build') 
      {
      steps {
      echo "building a maven project"
         sh 'mvn compile'
      }

}  
 stage ('test')
      {
      steps {
      echo "testing"
         sh 'mvn test'
      }

}  

 stage ('deploy')
      {
      steps {
      echo "deploy the project"
         sh 'mvn deploy'
      }

}  

}

}

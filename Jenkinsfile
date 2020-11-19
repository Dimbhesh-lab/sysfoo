pipeline{
  agent any
  
  tools{
    maven 'Maven 3.6.3'
  }

  stages{
   
   stage('Build'){
     steps{
       sh 'mvn compile'
     }
  }

  stages{

   stage('Unit Test'){
     steps{
       sh 'mvn clean test'
     }
  }

   stages{

   stage('Package'){
     steps{
       sh 'mvn package -DskipTest'
     }
  }
}

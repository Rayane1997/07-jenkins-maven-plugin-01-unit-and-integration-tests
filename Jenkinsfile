pipeline{
    agent any
    tools {
          maven 'my-maven-3' 
      }
    stages{
           
         stage("Clean Up"){
            steps{
               sh 'mvn clean ';
            }            
        }
        stage("Compile it "){
            steps{
                  sh 'mvn compile ';  
            }            
        }
        stage("Unit Tests "){
            steps{
                sh 'mvn test ';  
            }            
        }
         stage("Package (i.e. Generale the deployable JAR)"){
            steps{
                sh 'mvn package ';  
            }            
        }
    }
   
}
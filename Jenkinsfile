pipeline{
    agent any
    stages{
        stage("Checkout Code from SCM"){
            steps{
               
              git url: 'https://github.com/mromdhani/jenkins-maven-plugin-01-simplepipline',
                  branch: 'master'
               
            }            
        }
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
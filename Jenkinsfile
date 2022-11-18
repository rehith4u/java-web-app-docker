pipeline{
    agent any
    
    tools{
        maven "maven_3.8.6"
         }
    
    stages{
        
        stage('CheckoutCode'){
            steps{
                git credentialsId: '91edc316-755e-4ca5-bc0c-6f8ca064e04e', url: 'https://github.com/rehith4u/java-web-app-docker.git'
                 }
        }
    
        stage('Build'){
            steps{
                sh "mvn clean package"
                 }
        }
  /*      
        stage('ExecuteSonarQubeReport'){
            steps{
                sh "mvn sonar:sonar"
                 }
        }
  */
    }
}

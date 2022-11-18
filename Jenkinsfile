pipeline{
    agent any
    
   
    
    stages{
        
        stage('CheckoutCode'){
            steps{
                git credentialsId: 'Git_Credentials', url: 'https://github.com/rehith4u/java-web-app-docker.git'                 }
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

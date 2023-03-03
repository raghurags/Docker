pipeline{
    
    agent any
    tools {
    	maven 'MAVEN_HOME'
    } 
    stages {
        
        stage('Git Checkout'){
            
            steps{
                
                script{
                    
                    git branch: 'main', url: 'https://github.com/raghurags/Docker.git'
                }
            }
        }
        stage('Maven build'){
            
            steps{
                
                script{
                    
                    sh '/opt/apache-maven-3.6.3/bin/mvn clean install'
                }
            }
        }
        
  }
}

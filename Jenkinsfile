pipeline{
    agent any
    tools{
        
        maven 'mavenpath'
        jdk 'javapath'
        
    }
    stages{
        stage(gitcheckout){
            steps{
                git 'https://github.com/prasannalakshmi006/warproject.git'
            }
        }
        stage(package){
            steps{
               sh 'mvn clean package'
   
               }
        }  
      stage(deploywarfile){
           steps{
              sh '/opt/deploy.sh'
              }
          }
     } 
        
    }


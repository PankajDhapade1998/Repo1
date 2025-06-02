@Library("Shared") _
pipeline{
    
    agent any 

    
    stages{
        
        stage('clean ws'){
            steps{
                cleanWs()
            }
        }

        stage('from github scm'){
            steps{
                  echo "commiting from github"
                }
        }
        
        stage('Hello'){
            steps{
                script{
                    hello()
                }
            }
        }
        
        stage('clone'){
            steps{
                script{
                    clone("https://github.com/PankajDhapade1998/Scripting.git","master")
                }
            }
        }
        
        stage('custom function'){
            steps{
                script{
                    custom("Pankaj","Dhapade")
                }
            }
        }
        
          
        
    }
}

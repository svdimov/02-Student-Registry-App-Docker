pipeline{
    agent any
     
    
    stages{
        stage("Install dependencies"){
             steps{
                bat "npm install"
            }
           
        }
        stage(Testing){
            parallel{
                stage("Unit Testing"){
                    steps{
                        bat "npm audit"
                    }
                }
                stage("Integration Testing"){
                    steps{
                        bat "npm run test"
                    }
                }
            }
        }
       

}}
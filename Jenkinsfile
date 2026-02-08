pipeline{
    agent{
        label "node"
    }
    stages{
        stage("Install dependencies"){
             steps{
                bat "npm install"
            }
           
        }
        stage("Run tests"){
             steps{
                bat "npm test"
            }
        }
    }

}
pipeline {
    agent any
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/Kaiz78/laravelDocker", branch: "main"
            }
        }
        stage("Deploy") {
            environment {
                MY_PASSWORD = '21317c5b058dc3df379ea75f983bfacd88cb9caaa2697b32c0f2a43a6400bcedf12f3a0e006feaf7bdb3d13c4fbe96bee5cc34a9a072b63a290e0551ef960ea16e95c989af36e208a64c38c76972d7f258d6ad53'
            }
            steps{
               sh "echo $MY_PASSWORD | sudo -S touch /home/ubuntu/test.txt"
            }
        }
    }
}

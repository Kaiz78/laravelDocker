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
                MY_PASSWORD = credentials('2')
            }
            steps{
               sh "echo \$MY_PASSWORD | sudo -S touch /home/ubuntu/test.txt"
            }
        }
    }
}

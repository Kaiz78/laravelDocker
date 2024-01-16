pipeline {
    agent any
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/Kaiz78/laravelDocker", branch: "main"
            }
        }
        stage("Move project to the current working directory") {
            steps{
               sh "mv la /var/www/"
            }
        }
        stage("Delete") {
            steps{
               sh "cd .." 
               sh "rm -rf la"
               sh "rm -rf la@tmp"
            }
        }
    }
}

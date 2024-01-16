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
               sh "rsync -a ../la/ /var/www/la/"
               sh "rm -rf ../la" 
            }
        }
    }
}

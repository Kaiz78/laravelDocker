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
               sh "rsync -a ../laravelDocker/ /var/www/laravelDocker/" 
            }
        }
        stage("Build Project") {
            steps{
               sh "cd /var/www/la/ && docker-compose up -d --build"
            }
        }


    }
}

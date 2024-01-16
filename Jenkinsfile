pipeline {
    agent any
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/Kaiz78/laravelDocker", branch: "main"
            }
        }
        stage("Build Project") {
            steps{
               sh "docker-compose up -d --build"
            }
        }
        stage("Move project to the current working directory") {
            steps{
               sh "rsync -a ../laravelDocker/ /var/www/laravelDocker/" 
            }
        }


    }
}

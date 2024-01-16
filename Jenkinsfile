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
               sh "echo 4tc8*3pWcV-}4E | sudo docker-compose up -d --build"
            }
        }

    }
}





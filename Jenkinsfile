pipeline {
    agent {label: "dev"}
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

    }
}





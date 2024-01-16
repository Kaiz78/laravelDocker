pipeline {
    agent any
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/Kaiz78/laravelDocker", branch: "main"
            }
        }
        stage("Build Project") {
            environment {
                MY_PASSWORD = '4tc8*3pWcV-}4E'
            }
            steps{
                sh "echo \$MY_PASSWORD | sudo -S docker-compose up -d --build"
            }
        }

    }
}

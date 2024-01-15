pipeline {
    agent any
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/Kaiz78/laravelDocker", branch: "main"
            }
        }
        stage("Deploy") {
            steps{
                sh "cd /var/"
                sh "touch test.txt"
            }
        }
    }
}

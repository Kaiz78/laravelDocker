pipeline {
    agent {label "dev"}
    stages{
        stage("Clone Code"){
            steps{
                git url: "https://github.com/Kaiz78/laravelDocker", branch: "main"
            }
        }
        stage("Deploy") {
            steps{
                sh "pwd"
            }
        }
        stage("Deploy2") {
            steps{
                sh "touch text.php"
            }
        }
    }
}

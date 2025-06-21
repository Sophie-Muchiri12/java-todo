pipeline{
    agent any
    tools{
        gradle "gradle"
    }
    stages{
        stage("Clone Repo"){
            steps{
                git branch: "master", url: "https://github.com/Sophie-Muchiri12/java-todo.git"
            }
        }
        
        stage("Build code"){
            steps{
                sh "gradle build"
            }
        }
    }
}
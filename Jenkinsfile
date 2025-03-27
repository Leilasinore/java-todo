pipeline{
    agent any
    tools{gradle "gradle"}
    stages{
        stage("cloning repo"){
            steps{
                git branch:"master",url:"https://github.com/Leilasinore/java-todo.git"
            }
        }
        stage("building"){
            steps{
                sh "gradle build"
            }
        }
        stage("testing"){
            steps{
                sh "gradle test"
            }
        }
    }
}
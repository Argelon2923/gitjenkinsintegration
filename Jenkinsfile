pipeline {
    agent any 
    stages{
        stage("Git clone"){
            steps{
                git 'git@github.com:Argelon2923/gitjenkinsintegration.git'
            }
        }
        stage("Maven Test"){
            steps{
                sh "mvn test"
            }
        }
        stage("Maven Build"){
            steps{
                sh "mvn build"
            }
        }
         stage("Maven Deploy"){
            steps{
                echo "Deploying the war file to the server"
            }
        }
    }
}

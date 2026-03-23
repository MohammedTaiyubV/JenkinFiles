pipeline{
    agent any

    stages{

        stage("clone"){
            steps{
                git 'https://github.com/MohammedTaiyubV/Maven_Sample_Project.git'
            }
        }

        stage("build"){
            steps{
                sh 'mvn clean package'
            }
        }

        stage("execute"){
            steps{
                sh 'java -jar target/*.jar'
            }
        }
        stage("clone2"){
            steps{
                git 'https://github.com/MohammedTaiyubV/Maven_Project2.git'
            }
        }
        stage("build2"){
            steps{
                sh 'mvn clean package'
            }
        }
        stage("execute2"){
            steps{
                sh 'java -jar target/*.jar'
            }
        }
    }
}

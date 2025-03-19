pipeline{
    agent any
    environment{
        JAVA_HOME="C:\Program Files\Java\jdk-21"
        PATH="${JAVA_HOME}\\bin;${env.PATH}"
    }
    stages{
        stage('clone repo'){
            steps{
                   git branch: 'main' , url: 'https://github.com/User-coder07/Gojooo-.git',credentialsId: 'pr'
            }
        }
        stage('compile java'){
            steps{
                   git 'javac file1.java'
            }
        }
        stage('run java code'){
            steps{
                   git 'java file1'
            }
        }
    }
}

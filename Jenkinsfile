pipeline {
    agent any

    stages {

        stage('Build'){
            steps{
                sh 'javac tempJava.java tempJavaTest.java'
            }
        }

        stage('Test'){
            steps{
                sh 'java tempJavaTest'
            }
        }

        stage('Deploy'){
            steps{
                sh 'mkdir -p /home/ubuntu/deploy'
                sh 'cp *.class /home/ubuntu/deploy/'
            }
        }

    }
}
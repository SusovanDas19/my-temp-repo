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
          sh 'mkdir -p deploy'
          sh 'cp *.class deploy/'
        }
}

    }
}
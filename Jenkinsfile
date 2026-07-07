pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Compile') {
            steps {
                sh 'javac Test.java'
            }
        }

        stage('Run') {
            steps {
                sh 'echo -e "10\n20\n" | java Test'
            }
        }
    }
}
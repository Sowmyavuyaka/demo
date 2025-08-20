pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Cloning repository...'
                checkout scm
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling Java program...'
                sh 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running program...'
                sh 'java HelloWorld'
            }
        }
    }
}

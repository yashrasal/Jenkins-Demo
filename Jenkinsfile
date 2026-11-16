
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/yashrasal/Jenkins-Demo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Compiling Java Program...'
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Executing Java Program...'
                bat 'java HelloWorld'
            }
        }
    }
}

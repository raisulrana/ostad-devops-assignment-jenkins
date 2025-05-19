pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Print hello.txt') {
            steps {
                script {
                    def txt = readFile('hello.txt')
                    echo "hello.txt content:\n${txt}"
                }
            }
        }
    }
}


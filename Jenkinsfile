pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'env > env.txt'
                for (String i : readFile('env.txt').split("\r?\n")) {
                    println i
                }
                sh 'npm install'
            }
        }
    }
}

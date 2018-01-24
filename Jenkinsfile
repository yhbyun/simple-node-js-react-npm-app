pipeline {
    agent {
        docker {
            image 'ubuntu:16.04'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh "whoami"
            }
        }
    }
}

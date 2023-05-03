pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t python-webapp .'
            }
        }
        stage('Run') {
            steps {
                sh 'docker run -p 5000:5000 python-webapp'
            }
        }
    }
}


pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t jenkins-nginx .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker-compose up -d web'
            }
        }
    }
}

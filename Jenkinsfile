pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'sh docker build --no-cache -t jenkins-nginx .'

            }
        }

        stage('Run Container') {
            steps {
                sh 'docker-compose up -d web'
            }
        }
    }
}

pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main',
                url: 'https://github.com/cskarthi2752/car-website-1.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                rm -rf /var/www/html/*
                cp -r * /var/www/html/
                '''
            }
        }
    }
}

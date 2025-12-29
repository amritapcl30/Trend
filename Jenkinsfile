pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/amritapcl/trend-devops.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t trend-frontend .'
            }
        }
    }
}

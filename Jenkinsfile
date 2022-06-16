pipeline {
    agent any

    stages {
        stage('Checkout codes') {
            steps {
                echo 'Checking out codes from GIT repo'
                git branch: 'main', url: 'https://github.com/nguyencuongabcxyz/daddy_deployment.git'
            }
        }        
        stage('Deploy') {
            steps {
                echo 'Deploying the application'
                bat 'docker-compose up'
            }
        }
    }
}
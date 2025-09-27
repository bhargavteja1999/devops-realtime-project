pipeline {
    agent any

    environment {
        DOCKER_HUB_REPO = "bhargavteja14/inner_peace"  
        IMAGE_TAG = "latest"
    }

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/bhargavteja1999/devops-realtime-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("${bhargavteja14/inner_peace}:${latest}")
                }
            }
        }

        stage('Push to DockerHub') {
            steps {
                script {
                    docker.withRegistry('https://index.docker.io/v1/', 'dockerhub-credentials') {
                        docker.image("${bhargavteja14/inner_peace}:${latest}").push()
                    }
                }
            }
        }
    }
}

pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                echo 'Step 1: building the docker image from the Dockerfile'
                sh 'docker build -t my-nginx-app .'
            }
        }

        stage('Run the Container') {
            steps {
                echo 'Step 2: running the container on port 80'
                sh 'docker run -d --name my-nginx-app -p 80:80 my-nginx-app || echo "container might already be running"'
            }
        }

    }
}


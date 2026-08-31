pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Code checked out from Git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'chmod +x app.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running application test...'
                sh './app.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                echo 'Deployment successful!'
            }
        }
    }
}

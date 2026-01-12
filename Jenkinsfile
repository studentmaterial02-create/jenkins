pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/studentmaterial02-create/jenkins.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage running'
            }
        }
    }

    post {
        success {
            echo 'Pipeline SUCCESS'
        }
        failure {
            echo 'Pipeline FAILED'
        }
    }
}

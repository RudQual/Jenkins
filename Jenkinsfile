pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage running'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests'
            }
        }

        stage('Deploy') {
            when {
                branch 'main'
            }
            steps {
                bat 'echo Deploying application'
            }
        }
    }
}

pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/<username>/MYselenium.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean'
            }
        }

        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}

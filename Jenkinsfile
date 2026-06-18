pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/sgayatrijadhav-hub/mavenSrc.git'
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

        stage('Run') {
            steps {
                echo 'Running Selenium Application'
                echo 'https://www.saucedemo.com'
            }
        }
    }
}

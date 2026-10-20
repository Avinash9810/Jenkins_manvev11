
pipeline {
    agent any

    tools {
        maven 'maven'
        jdk 'jdk27'
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Avinash9810/Jenkins_manvev11.git'
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

        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}

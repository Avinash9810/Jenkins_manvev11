pipeline {
    agent any
    tools{
        maven  'maven'
        jdk 'jdk27'
    }
    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/Avinash9810/Jenkins_manvev11.git'
            }
        }
        stage('Compile') {
            steps {
              sh "mvn compile"
            }
        }
        stage('test') {
            steps {
                sh "mvn test"
            }
        }
        stage('build') {
            steps {
                sh "mvn package"
            }
        }
        }
    }

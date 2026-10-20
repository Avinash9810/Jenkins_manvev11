
pipeline {
    agent any

    tools {
        maven 'maven'
        jdk 'jdk27'
    }

    stages {
        stage('Compile') {
            steps {
                dir('apache-maven-3.10.0') {
                    sh 'mvn compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('apache-maven-3.10.0') {
                    sh 'mvn test'
                }
            }
        }

        stage('Build') {
            steps {
                dir('apache-maven-3.10.0') {
                    sh 'mvn package'
                }
            }
        }
    }
}

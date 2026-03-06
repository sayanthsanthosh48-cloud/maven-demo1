pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/sayanthsanthosh48-cloud/maven-demo1.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}

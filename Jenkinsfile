pipeline {
    agent any

    tools {
        maven 'Maven3'      // Maven name configured in Jenkins Global Tool Configuration         // JDK configured in Jenkins
    }

    stages {

          stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }

    post {
        success {
            echo 'Build Successful'
        }
        failure {
            echo 'Build Failed'
        }
    }
}

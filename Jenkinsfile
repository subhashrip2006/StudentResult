pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'javac StudentResult.java'
                echo 'Build Successful'
            }
        }

        stage('Test') {
            steps {
                bat 'java StudentResult > output.txt'
                bat 'findstr /C:"Result: PASS" output.txt'
                echo 'Test Successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline Completed Successfully'
        }
        failure {
            echo 'Pipeline Failed'
        }
    }
}

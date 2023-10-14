pipeline {
    agent { node { label 'Agent1'} }

    stages {
        stage('Build') {

            echo "this the building state"
        }

        stage('Test') {
            echo "this is testing"
        }

        stage('Deploy') {
            echo "deploying"
        }

    }

    post {
        always {
            echo "job complete"
        }

        success {
            echo "build is success"
        }

        failure {
            echo "build is fail"
        }
    }
}
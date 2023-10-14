pipeline {
    agent { node { label 'Agent1'} }

    stages {
        stage('Build') {

            steps {
                echo "this the building state"
            }
        }

        stage('Test') {

            steps {
                echo "this is testing"

            }
            
        }

        stage('Deploy') {
            steps {
                echo "deploying"
            }
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
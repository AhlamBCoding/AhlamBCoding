pipeline {
    agent any

    parameters {
        string(
            name: 'ENV_NAME',
            defaultValue: 'staging',
            description: 'Environment name'
        )
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Checkout stage"
            }
        }

        stage('Build') {
            steps {
                echo "Build stage"
            }
        }

        stage('Test') {
            steps {
                echo "Test stage"
                echo "Running tests against environment: ${params.ENV_NAME}"
            }
        }
    }

    post {
        always {
            echo 'Done'
        }
    }
}

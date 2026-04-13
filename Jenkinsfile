 pipeline {
    agent any
        stages {
        stage('Checkout') {
            steps {
               echo 'Checkout'
            }
        }

        stage('Build & Test') {
            steps {
               echo 'Test'
            }
        }

        stage('Report') {
            steps {
                echo 'Generate Allure Report'
            }
        }
    }
}

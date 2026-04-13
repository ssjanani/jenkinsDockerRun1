 pipeline {
    agent any

    tools {
        maven 'Maven'
    }
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

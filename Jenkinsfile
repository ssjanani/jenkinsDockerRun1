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
         post {
        always {

      
            junit '**/target/surefire-reports/*.xml'
            allure([
                includeProperties: false,
                jdk: '',
                results: [[path: 'target/allure-results']]
            ])
        }
    }
}

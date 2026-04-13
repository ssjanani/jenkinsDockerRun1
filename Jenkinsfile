 pipeline {
    agent any

    tools {
        maven 'Maven'
    }
        stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/ssjanani/jenkinsDockerRun1.git'
            }
        }

        stage('Build & Test') {
            steps {
                sh 'mvn clean test'
            }
        }

        stage('Report') {
            steps {
                echo 'Generate Allure Report'
            }
        }
    }
}

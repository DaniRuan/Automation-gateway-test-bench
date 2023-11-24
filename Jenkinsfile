pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/DaniRuan/Automation-gateway-test-bench'
            }
        }
        stage('Build') {
            steps {
                bat 'echo System testing started...'
            }
        }
        stage('Test') {
            steps {
                bat 'pio test -vvv'
            }
        }
    }
}

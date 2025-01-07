pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
               git 'https://github.com/Rajimaruthi/jenkins.git'
                
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}

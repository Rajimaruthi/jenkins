pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git credentialsId: '1ae91a36-5f63-4e05-8c86-1742a0e4f2b7', 
                url: 'https://github.com/Rajimaruthi/jenkins.git',
                git branch: 'master'
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

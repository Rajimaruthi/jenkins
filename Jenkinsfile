pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
               git 'https://github.com/Rajimaruthi/jenkins.git'
                
            }
        }
        stage('build') {
            steps {
               sh "mvn clean package"
                
            }
        }
    }
}

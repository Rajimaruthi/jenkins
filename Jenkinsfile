pipeline {
    
    agent any 
    
    environment {
        IMAGE_TAG = "${BUILD_NUMBER}"
    }
    
    stages {
        
        stage('Checkout'){
           steps {
                git credentialsId: '1ae91a36-5f63-4e05-8c86-1742a0e4f2b7', 
                url: 'https://github.com/Rajimaruthi/jenkins.git' 
                branch: 'master'
           }
        }
    }
}

pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', url: 'https://github.com/SanyaSinha/Devops.git'
            }
        }
        stage('Deploy to XAMPP') {
            steps {
                // Create the build directory if it doesn't exist
                bat 'mkdir build'
                
                // Copy index.html to the XAMPP htdocs directory
                bat 'copy /Y build\\index.html "C:\\xampp\\htdocs"'
            }
        }
    }
}

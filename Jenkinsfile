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
                // Copy hello.html
                bat 'copy /Y hello.html "C:\\xampp\\htdocs"'
                // Copy namaste.html
                bat 'copy /Y namaste.html "C:\\xampp\\htdocs"'
            }
        }
    }
}

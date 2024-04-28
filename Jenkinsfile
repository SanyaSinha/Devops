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
                // Replace 'build/index.html' with the path to your HTML file relative to the Jenkins workspace
                bat 'xcopy /Y build/index.html "C:\\xampp\\htdocs"'
            }
        }
    }
}

pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/SanyaSinha/Devops.git'
            }
        }
        stage('Deploy to XAMPP') {
            steps {
                // Replace 'your_command' with the actual command you want to run
                sh 'start /B your_command'
            }
        }
    }
}

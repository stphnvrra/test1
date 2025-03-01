pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package' // Replace with 'npm install' or 'python setup.py' if needed
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test' // Replace with appropriate test command
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add deployment scripts here
            }
        }
    }
}

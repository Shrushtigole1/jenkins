pipeline {
    agent any { 
        label 'node'
    }
    tools {
        nodejs 'npm'
    }
    environment {
        Name = "Mantasha"
    }

    stages {
        stage('clone') {
            steps {
                echo 'Hello World'
                git branch: 'main', url: 'https://github.com/Shrushtigole1/jenkins.git'
            }
        }
         stage('build') {
            steps {
                echo 'Hello World'
                sh 'npm i'
            }
        }
         stage('building the artifact') {
            steps {
                echo 'Hello World'
                sh 'npm run build'
            }
        }
    }
}

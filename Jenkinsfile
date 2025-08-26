pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/Nareshdarlaa/GitjenkinsIntegrstions.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Compiling Java program...'
                bat 'javac sample.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Running Java program...'
                bat 'HelloWorld'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}

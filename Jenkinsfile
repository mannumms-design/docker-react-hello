pipeline {

    agent any

    tools {
        nodejs 'NodeJS-22'
    }

    stages {

        stage('Checkout') {
            steps {
                echo 'Repository checked out successfully'
            }
        }

        stage('Verify Environment') {
            steps {
                sh 'pwd'
                sh 'ls -la'
                sh 'git --version'
                sh 'java -version'
                sh 'node --version'
                sh 'npm --version'
            }
        }

        stage('Verify Project') {
            steps {
                sh 'test -f package.json && echo "package.json found"'
                sh 'test -f Dockerfile && echo "Dockerfile found"'
                sh 'ls src'
            }
        }

    }
}
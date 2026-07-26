pipeline {

    agent any

    stages {

        stage('Welcome') {

            steps {

                echo 'Welcome to Jenkins Pipeline'

            }

        }

        stage('System Information') {

            steps {

                sh 'pwd'
                sh 'whoami'
                sh 'java -version'
                sh 'git --version'
            }

        }

    }

}
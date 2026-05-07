pipeline {
    agent any

    stages {
        stage('Dev') {
            steps {
                echo 'I am in Dev'
                echo 'checking git version'
                sh 'git --version'
            }
        }
                stage('Staging') {
            steps {
                echo 'I am in staging'
                echo 'checking docker version'
                sh 'docker --version'
                sh 'docker pull nginx'
            }
        }
                stage('Production') {
            steps {
                echo 'I am in Prod'
                echo 'listing docker images'
                sh 'docker images'
            }
        }

    }
}

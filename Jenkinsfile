pipeline {
    agent any
    environment {
        DB_PASS = credentials('jenkins-app-db-pass')
    }
    stages {
        stage('Build') {
            steps {
                sh 'docker compose build'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker compose up -d'
            }
        }
    }
}

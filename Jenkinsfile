#!/usr/bin/env groovy

pipeline {

    agent { dockerfile true }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'docker compose up --build'
            }
        }
    }
}

#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            dockerfile true
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'docker compose up --build'
            }
        }
    }
}

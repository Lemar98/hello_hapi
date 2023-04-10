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
                #sh 'npm install'
                sh 'docker compose up --build'
            }
        }
    }
}

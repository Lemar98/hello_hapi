#!/usr/bin/env groovy

pipeline {

    agent any

    stages {
        stage('Building docker image') {
            steps {
                echo 'Building...'
                sh 'docker build -t hello_hapi/example:0.1'
            }
        }
        stage('Runnig docker container') {
            steps {
                echo 'Running...'
                sh 'docker run -t example'
            }
        }
    }
}

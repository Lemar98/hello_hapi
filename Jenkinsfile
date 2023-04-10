#!/usr/bin/env groovy

pipeline {

    agent any

    stages {
        stage('Building docker image') {
            steps {
                echo 'Building...'
                sh 'sudo docker build -t hello_hapi/example:0.1'
            }
        }
        stage('Runnig docker container') {
            steps {
                echo 'Running...'
                sh 'sudo docker run -t example'
            }
        }
    }
}

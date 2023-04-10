#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            #image 'node'
            #args '-u root'
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
        #stage('Test') {
        #    steps {
        #        echo 'Testing...'
        #        sh 'npm test'
        #    }
        #}
    }
}

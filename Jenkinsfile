pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "here i would install any npm package"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "here I would run any tests"'
                sh 'echo "For example lets run \" node app.js \" "'
                sh 'node app.js'
            }
        }
        stage('Deliver') {
            steps {
                sh 'echo "Here I would push the code to production"'
            }
        }
    }
}
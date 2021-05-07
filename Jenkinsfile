pipeline {
    agent any
    stages {
        stage('Cloning Git') {
            steps {
                git 'https://github.com/Felipe11114/node-hello'
            }
        }

        stage('Install npm'){
            steps {
                sh 'npm install'
            }
        }

        stage('build proyect') {
            steps {
                sh 'npm start index.js'
            }
        }
    }
}

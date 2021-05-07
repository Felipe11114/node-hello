pipeline {
    agent any
    tools {nodejs "NodeJs"}
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
        
        stage('Build'){
            steps {
                nodejs('NodeJs') {
                    sh 'node index.js'
                }
                
            }
        }
    }
}

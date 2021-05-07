pipeline {
    agent any
    tools{ nodejs "node"}
    stages {
        stage('Cloning Git') {
            steps {
                git 'https://github.com/Felipe11114/node-hello'
            }
        }

        stage('Build npm'){
            steps {
                npm command: 'npm start index.js'
            }
        }
    }
}

pipeline {
    agent any
    tools {nodejs "nodejs"}
    stages {
        stage('Cloning Git') {
            steps {
                git 'https://github.com/Felipe11114/node-hello'
            }
        }

        stage('Install npm'){
            steps {
                sh'npm install'
            }
        }
    }
}

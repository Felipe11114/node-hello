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
                nodejs(cacheLocationStrategy: executor(), nodeJSInstallationName: 'NodeJs') {
                    sh 'npm run start'
                }
            }
        }
    }
}

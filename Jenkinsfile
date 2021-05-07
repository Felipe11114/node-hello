pipeline {
    agent any
    stages {
        stage('Cloning Git') {
            steps {
                git 'https://github.com/Felipe11114/node-hello'
            }
        }

        stage('Build npm'){
            steps {
                nodejs( nodeJSInstallationName : ' Nodo 6.x ') {
                    npm command: 'npm start index.js'
                }
            }
        }
    }
}

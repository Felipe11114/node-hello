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
                npm command: 'npm install', workspaceSubdirectory: 'node-hello'
            }
        }
        
        stage('Build proyect npm'){
            steps {
                npm command: 'npm start', workspaceSubdirectory: 'node-hello'
            }
        }
    }
}

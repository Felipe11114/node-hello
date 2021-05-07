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
                nodejs(cacheLocationStrategy: workspace()) {
                    npm command: 'npm start index.js'
                }
            }
        }
    }
}

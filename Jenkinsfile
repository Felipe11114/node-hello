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
                env.NODEJS_HOME = "{tool 'Node 6.x' }"
                env.PATH = "{env.NODEJS_HOME} / bin: {env.PATH}" 
                sh'npm install'
            }
        }
    }
}

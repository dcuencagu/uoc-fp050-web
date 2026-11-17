pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t miapp:$BUILD_NUMBER .'
            }
        }
        stage('Verify') {
            steps {
                sh 'docker images | grep miapp'
            }
        }
    }
}

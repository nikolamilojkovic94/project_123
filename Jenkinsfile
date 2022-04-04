pipeline {
    agent none
    stages {
        stage('Test') {
            agent {
                docker {
                    image 'python:3.8-slim'
                }
            }
            steps {
                sh 'python3 hello_world.py'
            }
            post {
                success {
                    sh 'echo Works!'
                }
            }
        }
    }
}

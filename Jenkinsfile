agent any
    stages {
        stage('Cloning git') {
            steps {
                sh "echo clone"
            }
        }
        stage('Build docker image') {
            steps {
                script {
                    sh "echo build"
                }
            }
        }
        stage('Upload to dockerhub') {
            steps {
                script {
                    sh "echo upload"
                    }
                }
            }
        }
        stage('clean up') {
            steps {
                sh "echo cleanup"
            }
        }
    }

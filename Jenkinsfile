pipeline {
    agent any
    environment {
        EMP_ID = "12"
    }
    stages {
        stage('build') {
            steps {
                sh "echo build"
                sh "echo $EMP_ID"
            }
        }
        stage('compile') {
            steps {
                sh "echo compile"
            }
        }
    }
}

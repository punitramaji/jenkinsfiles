pipeline {
    agent any
    environment {
        EMP_ID = "12"
    }
    stages {
        stage('write') {
            steps {
               script {
                   def date = new Date()
                   def data = "Hello World\nSecond line" + date
                   writeFile(file: 'myfile.txt', text: data)
                   sh "ls -l"
               } 
            }
        }    
        stage('read') {
            steps {
                script {
                    def data = readFile(file: 'myfile.txt')
                }
            }
        }
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

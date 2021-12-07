pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh("pwd")
                sh("ls")
                sh("chmod 700 my.sh")
                script{
                    def me = sh (script: 'ls', returnStdout: true)
                    println me
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
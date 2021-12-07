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
                    def me = sh (script: './my.sh', returnStdout: true)
                    println me[0]
                    println me[1]
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
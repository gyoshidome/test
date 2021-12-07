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
                    println me
                    println me.split(',')
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

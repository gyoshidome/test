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
                me = sh (script: './my.sh', returnStdout: true)
                echo $me
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
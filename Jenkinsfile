pipeline {
    agent any

    stages {
        stage('rm old') {
            steps {
                sh 'rm -rf blablatest'
            }
        }
        stage('asdasd') {
            steps {
                sh 'git clone https://github.com/Zeekee7/blablatest.git'
            }
        }
        stage('copy') {
            steps {
                sh 'ls -l'
                sh 'cp blablatest/* /usr/share/nginx/html/'
            }
        }
    }
}

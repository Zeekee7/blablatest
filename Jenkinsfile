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
        stage('Deploy Prod') {
            when { env.BRANCH_NAME == 'master'} 
            steps {
                echo 'I only execute on the master branch'
            } 
        }
    }
}

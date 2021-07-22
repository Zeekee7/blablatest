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
            if (env.BRANCH_NAME == 'master') {
                echo 'I only execute on the master branch'
            } else {
                echo 'I execute elsewhere'
            }
        }
    }
}

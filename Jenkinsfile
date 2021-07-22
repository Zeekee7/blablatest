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
        stage('Deploy NonProd') {
            when { expression { env.BRANCH_NAME != 'master'} }
            steps {
                echo 'Deploy to non prod env'
                sh 'cp blablatest/test.html /usr/share/nginx/html/test/intex.html'
            } 
        }
        stage('Deploy Prod') {
            when { expression { env.BRANCH_NAME == 'master'} }
            steps {
                echo 'Deploy to production'
                input "Deploy to prod?"
                sh 'cp blablatest/test.html /usr/share/nginx/html/index.html'
            } 
        }
    }
}

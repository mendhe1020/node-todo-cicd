pipeline {
    agent any
    
    stages {
        stage('SCM Checkout A') {
            steps {
                echo 'SCM'
                git url: 'https://github.com/mendhe1020/node-todo-cicd.git'
            }
        }

        stage('Build') {
            steps {
                // Install npm dependencies
                sh 'npm i -f'
            }
        }

        stage('Deploy') {
            steps {
                // run pm2
                sh 'npm install pm2 --save-dev'
                sh 'sudo pm2 start /var/lib/jenkins/workspace/_Multibranch_Pipeline_Devlopment/app.js'
            }
        }
    }
}

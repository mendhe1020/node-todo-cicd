pipeline {
    agent { label "docker_slave"}
    
    stages {
        stage('SCM Checkout A') {
            steps {
                echo 'SCM'
                git url: 'https://github.com/mendhe1020/node-todo-cicd.git'
            }
        }
    }
}

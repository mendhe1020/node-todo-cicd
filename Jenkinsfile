pipeline {
    agent any
    
    stages {
        stage("Code") {
            steps {
                // Declarative syntax for checking out code from SCM
                checkout([$class: 'GitSCM', 
                          branches: [[name: '$GIT_BRANCH']], 
                          userRemoteConfigs: [[url: 'https://github.com/mendhe1020/node-todo-cicd.git']]])
            }
        }
    }
}

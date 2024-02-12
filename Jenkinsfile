pipeline {
    agent any
    
    stages {
        stage("Checkout") {
            steps {
                // Checkout the code from the Git repository
                git branch: '$GIT_BRANCH', url: 'https://github.com/mendhe1020/node-todo-cicd.git'
            }
        }
    
    }
}

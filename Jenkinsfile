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
        stage("Build") {
            steps {
                // Example: Building a Node.js project
                sh 'npm install'
            }
        }
        stage("Test") {
            steps {
                // Example: Running tests for a Node.js project
                sh 'npm test'
            }
        }
        stage("Deploy") {
            steps {
                // Example: Deploying a Node.js project
                sh 'npm run deploy'
            }
        }
    }
}

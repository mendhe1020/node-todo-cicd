pipeline {
    agent any
    
    stages {
        stage("Checkout") {
            steps {
                // Checkout the code from the Git repository
                git branch: '$GIT_BRANCH', url: 'https://github.com/mendhe1020/node-todo-cicd.git'
            }
        }
        
        stage("Build") {
            steps {
                // Build your project
                sh 'npm install' // Assuming it's a Node.js project
            }
        }
        
        stage("Test") {
            steps {
                // Run tests for your project
                sh 'npm test' // Assuming you have tests to run
            }
        }
        
        stage("Deploy") {
            steps {
                // Deploy your project
                sh 'npm run deploy' // Assuming you have a deployment script
            }
        }
    }
}

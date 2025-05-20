pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *') // Poll GitHub every 2 mins
    }

    stages {
        stage('Build') {
            steps {
                echo "Building the code using Maven"
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "Running tests using Mocha and Chai"
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Analyzing code with ESLint"
            }
        }

        stage('Security Scan') {
            steps {
                echo "Scanning vulnerabilities with npm audit"
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploying to AWS EC2 staging server"
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests in staging with Newman"
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying to AWS EC2 production server"
            }
        }
    }
}




pipeline {
    agent any

    stages {
        stage('install-pip-deps') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/mtararujs/python-greetings'

                echo 'Checking repository contents...'
                sh 'ls'

                echo 'Installing Python pip dependencies...'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('deploy-to-dev') {
            steps {
                echo 'Deploying to Development...'
                
            }
        }

        stage('tests-on-dev') {
            steps {
                echo 'Running tests on Development...'
               
            }
        }

        stage('deploy-to-staging') {
            steps {
                echo 'Deploying to Staging...'
            }
        }

        stage('tests-on-staging') {
            steps {
                echo 'Running tests on Staging...'
            }
        }

        stage('deploy-to-preprod') {
            steps {
                echo 'Deploying to Pre-production...'
            }
        }

        stage('tests-on-preprod') {
            steps {
                echo 'Running tests on Pre-production...'
            }
        }

        stage('deploy-to-prod') {
            steps {
                echo 'Deploying to Production...'
            }
        }

        stage('tests-on-prod') {
            steps {
                echo 'Running tests on Production...'
            }
        }
    }
}


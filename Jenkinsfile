pipeline {
    agent any

    stages {
        stage('install-pip-deps') {
            steps {
                echo 'Cloning repository...'
                git 'https://github.com/rtwork321/python-greetings.git'
                bat 'ls' 
                bat 'pip3 install -r requirements.txt' // Installing dependencies
    }
}


        stage('deploy-to-dev') {
            steps {
                echo 'Deploying to Development...'
                // sh 'git clone https://github.com/mtararujs/python-greetings'
                // sh 'cd python-greetings'
                // sh 'pm2 delete greetings-app-dev || true'
                // sh 'pm2 start app.py --name greetings-app-dev -- --port 7001'
            }
        }

        stage('tests-on-dev') {
            steps {
                echo 'Running tests on Development...'
                // sh 'git clone https://github.com/mtararujs/course-js-api-framework'
                // sh 'cd course-js-api-framework'
                // sh 'npm install'
                // sh 'npm run greetings greetings_dev'
            }
        }

        stage('deploy-to-staging') {
            steps {
                echo 'Deploying to Staging...'
                // sh 'git clone https://github.com/mtararujs/python-greetings'
                // sh 'cd python-greetings'
                // sh 'pm2 delete greetings-app-staging || true'
                // sh 'pm2 start app.py --name greetings-app-staging -- --port 7002'
            }
        }

        stage('tests-on-staging') {
            steps {
                echo 'Running tests on Staging...'
                // sh 'git clone https://github.com/mtararujs/course-js-api-framework'
                // sh 'cd course-js-api-framework'
                // sh 'npm install'
                // sh 'npm run greetings greetings_staging'
            }
        }

        stage('deploy-to-preprod') {
            steps {
                echo 'Deploying to Pre-production...'
                // sh 'git clone https://github.com/mtararujs/python-greetings'
                // sh 'cd python-greetings'
                // sh 'pm2 delete greetings-app-preprod || true'
                // sh 'pm2 start app.py --name greetings-app-preprod -- --port 7003'
            }
        }

        stage('tests-on-preprod') {
            steps {
                echo 'Running tests on Pre-production...'
                // sh 'git clone https://github.com/mtararujs/course-js-api-framework'
                // sh 'cd course-js-api-framework'
                // sh 'npm install'
                // sh 'npm run greetings greetings_preprod'
            }
        }

        stage('deploy-to-prod') {
            steps {
                echo 'Deploying to Production...'
                // sh 'git clone https://github.com/mtararujs/python-greetings'
                // sh 'cd python-greetings'
                // sh 'pm2 delete greetings-app-prod || true'
                // sh 'pm2 start app.py --name greetings-app-prod -- --port 7004'
            }
        }

        stage('tests-on-prod') {
            steps {
                echo 'Running tests on Production...'
                // sh 'git clone https://github.com/mtararujs/course-js-api-framework'
                // sh 'cd course-js-api-framework'
                // sh 'npm install'
                // sh 'npm run greetings greetings_prod'
            }
        }
    }
}

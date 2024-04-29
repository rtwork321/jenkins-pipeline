pipeline {
    agent any

    stages {
        stage('install-pip-deps') {
            steps {
                echo 'Cloning repository...'
                git branch: 'main', url: 'https://github.com/rtwork321/python-greetings.git'
                bat 'dir' 
                bat 'pip3 install -r requirements.txt' // Installing dependencies
    }
}
        stage('deploy-to-dev') {
            steps {
                echo 'Deploying to Development...'
                git branch: 'main', url: 'https://github.com/rtwork321/python-greetings.git'
                bat 'pm2 delete greetings-app-dev || true'
                //bat 'pm2 start app.py --name greetings-app-dev -- --port 7001'
                script {
                    bat 'python app.py &'
                    bat 'timeout /t 5 /nobreak > NUL'
                    bat 'netstat -ano | findstr :7001'
                }            
            }
        }

        stage('tests-on-dev') {
            steps {
                echo 'Running tests on Development...'
                git branch: 'main', url: 'https://github.com/rtwork321/course-js-api-framework.git'
                bat 'npm install'
                bat 'npm run greetings greetings_dev'
                //bat 'npm run greetings_dev'
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

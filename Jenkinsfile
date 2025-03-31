pipeline {
    agent any
     triggers {
        cron('0 9 * * 1-5')
        pollSCM('H/5 * * * *')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Your build commands here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Your test commands here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Your deployment commands here
            }
        }
    }
}

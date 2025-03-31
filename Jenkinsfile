pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/YourRepo/website.git'
            }
        }

        stage('Deploy HTML') {
            steps {
                script {
                    def webDir = 'C:\\xampp\\htdocs\\'
                    bat "copy index.html ${webDir}"
                    echo "HTML file deployed to web server!"
                }
            }
        }
    }
}

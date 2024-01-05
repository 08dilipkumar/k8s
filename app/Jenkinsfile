pipeline {
    agent any

    stages {
        stage('CLONE') {
            steps {
                git branch: 'main', url: 'https://github.com/08dilipkumar/php.git'
            }
        } 
        stage('DEPLOY') {
            steps {
                sh 'cp main.php /var/www/html'
            }
        }
    }
}

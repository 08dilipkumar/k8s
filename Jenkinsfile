pipeline {
    agent any

    stages {
        stage('CLONE') {
            steps {
                git branch: 'main', url: 'https://github.com/08dilipkumar/k8s.git'
            }
        } 
        stage('DEPLOY') {
            steps {
                sh 'scp index.php root@172.17.0.2:/var/www/html'
            }
        }
    }
}

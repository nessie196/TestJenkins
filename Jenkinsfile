pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    pwd
                    whoami
                    composer --version
                    cd /var/www/test
                    composer install
                    cp .env.example .env
                    php artisan key:generate
                '''
            }
        }
    }
}
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
                    git pull --force origin master
                    git reset --hard origin/master
                    composer install
                    cp .env.example .env
                    php artisan key:generate
                '''
            }
        }
    }
}
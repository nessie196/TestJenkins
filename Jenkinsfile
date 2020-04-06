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
                    git reset --hard origin/master
                    git pull --force origin master
                    composer install
                    cp .env.example .env
                    php artisan key:generate
                '''
            }
        }
    }
}
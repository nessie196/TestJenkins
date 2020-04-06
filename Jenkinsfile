pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    echo "Multiline shell steps works too"
                    pwd
                    whoami
                    ls -lah
                    composer --version
                    composer install
                    cp .env.example .env
                    cd /var/www/test
                    ls -lah
                '''
            }
        }
    }
}
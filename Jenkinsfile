pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    echo "Multiline shell steps works too"
                    cd ..
                    pwd
                    ls -lah
                    composer --version
                    cd /var/www/test
                    ls -lah
                '''
            }
        }
    }
}
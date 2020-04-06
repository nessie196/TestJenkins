pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    echo "Multiline shell steps works too"
                    cd /var/www
                    ls -lah
                '''
            }
        }
    }
}
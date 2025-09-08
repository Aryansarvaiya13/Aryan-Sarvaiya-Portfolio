pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/Aryansarvaiya13/Aryan-Sarvaiya-Portfolio.git'
            }
        }

        stage('Deploy to Nginx') {
    steps {
        sh '''
        echo "Deploying portfolio to Nginx..."
        sudo rm -rf /var/www/html/*
        sudo cp -r * /var/www/html/
        '''
            }
        }

    }
}

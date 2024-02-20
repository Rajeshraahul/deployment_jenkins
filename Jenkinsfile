pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                sh '''
                cp ./jenkins.pem ~/.ssh/
                cp ./config ~/.ssh/
                cd ~/.ssh/
                ssh 54.227.159.255
                '''
                // yes |sudo apt-get install git 
                // yes |sudo apt-get install apache2
            }
        }
    }
}
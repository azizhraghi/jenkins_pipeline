pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('Checkout GIT') {
            steps {
                echo 'Pulling...'
                git branch: 'main',
                    url: 'https://github.com/azizhraghi/jenkins_pipeline.git'
            }
        }
        stage('Show Date') {
            steps {
                sh 'date'
            }
        }
    }
}

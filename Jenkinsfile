pipeline{
    agent any
    triggers{
        cron('*/2 * * * *')
    }

    stages{
        stage('checkout code'){
            steps{
                checkout scm
            }
        }
        stage('run python program'){
            steps{
                sh 'python3 extract.py'
            }
        }

    }
}
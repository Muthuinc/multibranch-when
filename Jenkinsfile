pipeline {
    agent any

    stages {
        stage('master') {
            when {
                expression { branch 'master' }
            }
            steps {
                echo 'main branch'
            }
        }
        stage('Main 1') {
            when {
                expression { branch 'master' }
            }
            steps {
                echo 'main 1'
            }
        }

        stage('Dev') {
            when {
                expression { branch 'Dev' }
            }
            steps {
                echo 'Dev branch'
            }
        }
        stage('Dev 1') {
            when {
                expression { branch 'Dev' }
            }
            steps {
                echo 'Dev 1'
            }
        }
    }
}

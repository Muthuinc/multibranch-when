pipeline {
    agent any

    stages {
        stage('master') {
            when {
                branch 'master'
            }
            steps {
                echo 'main branch'
            }
        }
        stage('Main 1') {
            when {
                branch 'master' // This is correct since there is only a "master" branch
            }
            steps {
                echo 'main 1'
            }
        }

        stage('Dev') {
            when {
                branch 'Dev'
            }
            steps {
                echo 'Dev branch'
            }
        }
        stage('Dev 1') {
            when {
                branch 'Dev'
            }
            steps {
                echo 'Dev 1'
            }
        }
    }
}

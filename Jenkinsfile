pipeline {
    agent any

    stages {
        stage('master') {
            when {
                branch 'master'
            }
            steps {
                sh """
                echo 'main branch'
                """
            }
        }
        stage('Main 1') {
            when {
                 branch 'master' 
            }
            steps {
                sh """
                echo 'main 1'
                """
            }
        }

        stage('Dev') {
            when {
                branch 'Dev' 
            }
            steps {
                sh """
                echo 'Dev branch 1'
                """
            }
        }
        stage('Dev 1') {
            when {
                 branch 'Dev' 
            }
            steps { 
                sh """
                echo 'Dev 1'
                """
            }
        }

        stage('master') {
            when {
                branch 'master'
            }
            steps {
                sh """
                echo 'main branch'
                """
            }
        }

        stage('Dev 1') {
            when {
                 branch 'Dev' 
            }
            steps { 
                sh """
                echo 'Dev 1'
                """
            }
        }
    }
}

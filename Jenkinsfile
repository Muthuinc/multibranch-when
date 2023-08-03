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
                changelog 'm.sh'
            }
            steps {
                sh """
                ./m.sh
                """
            }
        }
        stage('Dev 1') {
            when {
                 changelog 'm.sh' 
            }
            steps { 
                sh """
                echo 'Dev 1'
                """
            }
        }

        stage('masterr') {
            when {
                equals(actual: currentBuild.number, expected: 10)
            }
            steps {
                sh """
                echo 'main'
                """
            }
        }

        stage('Devr 1') {
            when {
                 branch 'Dev' 
            }
            steps { 
                sh """
                echo 'De'
                """
            }
        }
    }
}

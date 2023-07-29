Pipeline {
    agent any

    stages {
        stage ('Main') {
            when {
                branch 'main'
            }
            steps {
                echo 'main branch'
            }
        }
        stage ('Main 1') {
            when {
             branch 'main'
            }
            steps {
                echo 'main 1'
            }
        }

        stage ('Dev') {
            when {
                branch 'Dev'
            }
            steps {
                echo 'Dev branch'
            }
        }
        stage ('Dev 1') {
            when {
             branch 'Dev'
            }
            steps {
                echo 'Dev 1'
            }
        }
    }
}

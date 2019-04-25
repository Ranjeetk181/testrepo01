pipeline {
    agent 'any'
    stages {
        stage('Deliver for development') {
            when {
                branch 'dev'
            }
            steps {
                sh 'echo "this is dev branch"'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'master'
            }
            steps {
                sh 'echo "thsi is master branch"'
            }
        }
    }
}

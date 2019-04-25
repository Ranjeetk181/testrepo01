pipeline {
    agent 'any'
    stages {
        stage('Testing') {
            steps {
                sh 'echo "YOu can write test cases here"'
               
            }
        }
        stage("Unit-testing") {
            steps {
                parallel (
                    "firstTask" : {
                     sh 'echo "First unit test"'
                    },
                    "secondTask" : {
                    sh 'echo "Second unit test"'
                    }
                    )
             }
        }
    }
}

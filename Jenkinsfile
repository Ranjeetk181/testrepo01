pipeline {
    agent 'any'
    parameters {
        string(name: 'environmnt', defaultValue: 'xyz', description: 'define the enviroment')
    }
    environment {
        MY_ENV = "mytesting"
    }
    stages {
        stage('Testing') {
            steps {
                sh 'echo "YOu can write ${params.environmnt} cases here"'
               
            }
        }
        stage('Deployment') {
            steps {
                sh 'echo "YOu can write deployment steps for ${env.MY_ENV}."'
                }
        }
    }
}

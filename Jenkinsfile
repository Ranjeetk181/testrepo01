pipeline {
    agent 'any'
    parameters {
        string(name: 'ENVIRON', defaultValue: 'xyz', description: 'define the enviroment')
    }
    environment {
        MY_ENV = 'mytesting'
    }
    stages {
        stage('Testing') {
            steps {
                echo "YOu can write ${params.ENVIRON} cases here"
               
            }
        }
        stage('Deployment') {
            steps {
                echo "YOu can write deployment steps for ${env.MY_ENV}."
                }
        }
    }
}

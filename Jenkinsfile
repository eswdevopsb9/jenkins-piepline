pipeline {
    agent {
        label 'app-slave'
    }
    environment {
        //key=value
        DEPLOY_TO = 'Production'
    }
    stages {
        stage ('Printing data') {
            when {
                environment name: 'DEPLOY_TO', value: 'Dev'
                //branch validation
                //parameters based validation (100%)
            }
            steps {
                echo "*******Printing some data*********"
            }
        }
    }
}

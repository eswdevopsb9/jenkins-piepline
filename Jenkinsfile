pipeline {
    agent {
        label 'app-slave'
    }
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage ('DeployToDev') {
            steps {
            echo "Deploying to Dev environment"
            }
        }
        stage ('DeployToProd') {
            when {
                allOf {
                    branch 'production'
                    //expression when {BRANCH_NAME ==~ /(production|staging)/}
                    environment name: 'DEPLOY_TO', value: 'production'
                }
            }
            steps {
                echo "Deploying to Prod environment"
            }
        }
    }
}

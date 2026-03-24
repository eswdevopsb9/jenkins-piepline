pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "***Building the application***"
            }
        }
        stage ('Sonar') {
            steps {
                echo "***Running sonar scans***"
            }
        }
        stage ('DockerBuild&Push') {
            steps {
                echo "***Building and pushing Docker images***"
            }
        }
        stage ('DeployToDev') {
            steps {
                echo "***Deploying to Dev environment"
            }
        }
        stage ('DeployToTest') {
            steps {
                echo "***Deploying to Test environment***"
            }
        }
        stage ('DeployToStage') {
            steps {
                echo "***Deploying to Stage environment***"
            }
        }
        stage ('DeployToProd') {
            options {
                timeout(time:300, unit:'SECONDS') //set time for the approval step
            }
            input {
                message "Are you sure want to deploy to prod environment?"
                ok 'Yes'
                submitter 'i27academy', 'sreuser' //only users with these usernames can approve the deployment
            }
            steps {
                echo "***Deploying to Prod environment***"
            }
        }
    }
}

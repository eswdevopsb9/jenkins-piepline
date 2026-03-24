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
            steps {
                echo "***Deploying to Prod environment***"
            }
        }
    }
}

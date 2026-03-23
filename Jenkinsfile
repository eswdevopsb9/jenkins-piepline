pipeline {
    agent {
        label 'app-slave'
    }
    environment {
        DEPLOY_TO = 'Production'
    }
    stages {
        stage ('DevDeploy') {
            steps {
                echo "******Deploy in Dev Environment*******"
            }
        }
        stage ('ProdDeploy') {
            steps {
                echo "******Deploy in Prod Environment*******"
            }
        }
    }
}

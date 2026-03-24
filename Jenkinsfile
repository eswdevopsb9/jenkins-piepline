pipeline {
    agent {
        label 'app-slave'
    }
    stages {
        stage ('Example Build') {
            steps {
                echo "***Hello World***"
            }
        }
        stage ('Example Deploy') {
            when {
                expression {BRANCH_NAME ==~ /(production|staging)/}
            }
            steps {
                echo "***Deploying***"
            }
        }
    }
}

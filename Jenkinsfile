pipeline {
    agent any
    stages {
    }
    post {
        always {
            echo "***This always run regarless of the build result***"
        }
        success {
            echo "***This will run if the build is successful***"
        }
        failure {
            echo "***This will run if the build fails***"
        }
    }
}

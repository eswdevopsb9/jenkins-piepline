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
        stage ('ubuntu version') {
            steps {
                sh 'lsb_release'
            }
        }
    }
    post {
        always {
            echo "***This always run regardless of the build result***"
        }
        success {
            echo "***This will run if the build is successful***"
        }
        failure {
            echo "***This will run if the build fails***"
        }
    }
}

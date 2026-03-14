pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                retry (3) {
                    echo "This is a Retry example"
                    //replicate a failure
                     error "This is an error from Retry example"
                }
            }
        }
    }
}

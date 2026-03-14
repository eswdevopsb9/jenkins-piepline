pipeline {
    agent any
    stages {
        stage ('Build')
        steps {
            echo "This is a Retry example"
            //replicate a failure
            error "This is an error from Retry example"
        }
    }
}

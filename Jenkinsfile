pipeline {
    agent any
    stages {
        stage ('First stage') {
            steps {
            echo "************* Printing the hostname where this stage is running ************"
            sh 'hostname -i'
            }

        }
        stage ('Second stage'){
            steps {
            echo "************* Printing the hostname where this stage is running ************"
            sh 'hostname -i'
            }
        }
    }
}

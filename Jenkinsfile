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
            agent {
                label 'app-slave'
            }
            steps {
            echo "************* Printing the hostname where this stage is running ************"
            sh 'hostname -i'
            }
        }
    }
}

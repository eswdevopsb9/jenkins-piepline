//pipeline code
pipeline {
    agent {
        label 'app-slave'
    }
    stages {
        stage ('build') {
            steps {
                //I want to write some message
                echo "Hello from build step using piepline"
            }
        }
        stage ('hostname') {
            steps {
                sh 'hostname -i'
                // sh 'mvn package'
                // sh 'docker build'
            }
        }
    }
} 

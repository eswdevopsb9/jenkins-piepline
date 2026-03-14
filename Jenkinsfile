pipeline {
    agent any
    tools {
        //This name should match the name configured in tools section
        maven 'maven-3.8.9'
    }
    stages {
        stage (maven) {
            steps {
                echo "Welcome to Maven section printing maven version"
                sh 'mvn --version'
            }
        }
    }
}

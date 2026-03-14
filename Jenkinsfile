pipeline {
    agent any
    tools {
        //This name should match the name configured in tools section
        maven 'maven-3.8.9'
    }
    stages {
        stage (maven) {
            steps {
                echo "Welcome to Maven section, this is default java"
                sh 'mvn --version'
            }
        }
        stage (maven) {
            tools {
                java 'jdk-17'
            }
            steps {
                echo "Welcome to Maven section, this is custom java"
                sh 'mvn --version'
            }
        }
    }
}

pipeline {
    agent any
    tools {
        //This name should match the name configured in tools section
        maven 'maven-3.8.9'
    }
    stages {
        stage ('mavendefault') {
            steps {
                echo "Welcome to Maven section, this is default java"
                sh 'mvn --version'
            }
        }
        stage ('mavencustom') {
            tools {
                jdk 'jdk-17'
            }
            steps {
                echo "Welcome to Maven section, this is custom java"
                sh 'mvn --version'
            }
        }
    }
}

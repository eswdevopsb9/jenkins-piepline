pipeline {
    agent any
    environment {
        //key = value
        name = "Mahesh"
        course = "Docker and k8s"
    }
    stages {
        stage ('Build') {
            steps {
                echo "Welcome Mr ${name}"
                echo "You are enrolled for ${course} course"
                echo "${name} is certified in CKA"
            }
        }
    }
}

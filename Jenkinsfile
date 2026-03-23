pipeline {
    agent {
        label 'app-slave'
    }
    //global pipeline
    environment {
        name = "Eswar"
        course = "Docker and K8s"
    }
    stages {
        stage ('First stage') {
        //stage level pipeline
        environment {
            cloud = "AWS"
        }
        steps {
            echo "*********Welcome to ${name}*********"
            echo "*********You are enrolled for ${course} course*********"
            echo "*********You are certified in CKA*********"
            echo "*********${name} certified in ${cloud} cloud*********"
        }
        }
        stage ('Second stage') {
            environment {
                name = "Anitha"
                cloud = "GCP"
                }
                steps {
            echo "*********Welcome to ${name}*********"
            echo "*********You are enrolled for ${course} course*********"
            echo "*********You are certified CKA*********"
            echo "*********${name} certified in ${cloud} cloud*********"
        }
        }
    }
}

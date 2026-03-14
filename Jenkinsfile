pipeline {
    agent any
    stages {
        stage ('build stage') {
            steps {
                //Declarative code
                echo "This is a build stage"
                sh 'hostname -i'
            }
        }
        stage ('groovy stage'){
            steps {
                scripts {
                    //logic
                    //variable definition
                    //def variable = "value"
                    def course = "Kubernetes (k8s)"
                    //there are various ways to call variables
                    if (course == "Kubernetes (k8s)")
                    println("Thanks for enrolling into ${course} course")
                    else
                    println("Do enroll into ${course} course")
                }
            }
        }
    }
}

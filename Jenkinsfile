pipeline {
    agent {
        label 'app-slave'
    }
    parameters {
        string (
            name: 'PERSON',
            defaultValue: 'Eswar',
            description: 'Who should I say hello to?'
        )
        text (
            name: 'BIOGRAPHY',
            defaultValue: '',
            description: 'Enter some information about the person'
        )
        booleanParam ( //true or false
            name: 'TOGGLE',
            defaultValue: true,
            description: 'Toggle this value'
        )
        choice (
            name: 'CHOICE',
            choices: ['One', 'Two', 'Three'],
            description: 'Pick something'
        )
    }
    stages {
        stage ('printstage') {
            steps {
                echo "Welcome to ${params.PERSON}"
                echo "Your Biography is: ${params.BIOGRAPHY}"
                echo "You toggled ${params.TOGGLE}"
                echo "You have choosen ${params.CHOICE}"
            }
        }
    }
}

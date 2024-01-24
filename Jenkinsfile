pipeline {
    agent { node { label 'agent1' } }

    stages {
        stage('Build') {
            steps {
                echo 'Building....'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                //error 'this is failed'            
        }
    }
    post { 
        always { 
            echo 'I will always run weather the job is done or not'
        }
        success {
            echo 'i will run if it is success'
        }
        failure{
            echo 'i wll run if it failed'
        }
    }
}
}
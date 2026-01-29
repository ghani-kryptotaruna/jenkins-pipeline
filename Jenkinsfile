pipeline {
    agent {
        node {
            label "Windows && Linux"
        }
    }
    
    stages {
        
        stage ('Build') {
            steps {
                echo('Hallo Build')
            }
        }
    }

    stage ('Deplog') {
            steps {
                echo('Hallo Deploy')
            }
        }
    }

    post {
        always {
            echo 'I will always say Hello again!'
        }
        success {
            echo 'Yay success!'
        }
        failure {
            echo 'Oh no, failure!'
        }
        cleanup {
            echo "Don't care success or error"
        }
    }
}

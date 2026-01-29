pipeline {
    agent {
        node {
            label "Windows && Linux"
        }
    }
    stages {
        stage ('Hallo') {
            steps {
                echo('Hallo apa kabar')
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

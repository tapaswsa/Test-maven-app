pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
               echo "Build"
            }
        }
        stage ('Test') {
            steps {
               echo "Test"
            }
        }
        stage ('Deploy') {
            steps {
                echo "Deploy" 
            }
        }
    }
    post { 
        cleanup { 
            echo "Clean up in post workspace"
            cleanWs()
        }
    }
}      

    post { 
        cleanup { 
            echo "Clean up in post workspace"
            cleanWs()
        }
    }
}



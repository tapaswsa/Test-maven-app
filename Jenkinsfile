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
        
        stage ('Sonar Scan') {
            when {
                branch "feature/*"
            }
            steps {
                echo "Sonar" 
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

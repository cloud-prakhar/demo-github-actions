pipeline {
    
    agent any
    
    environment {
        APP_NAME = "Test-App"
        APP_VERSION = "1.0.0"
        APP_ENV = "dev"
    }
    
    stages {
        stage("Build") {
            steps {
                echo "Building Application..."
                echo "Building App with name ${APP_NAME}"
                echo "App version is ${APP_VERSION}"
            }
        }
        
        stage("Test") {
            steps {
                echo "Test Application..."
            }
        }
        
        stage("Deploy") {
            steps {
                echo "Deploy Application.."
            }
        }
    }
    
    post {
        success {
            echo "Pipeline is successfull"
        }
        
        failure {
            echo "This pipeline is failed"
        }
        
        always {
            echo "Whether success or fail, you should run"
        }
    }
}

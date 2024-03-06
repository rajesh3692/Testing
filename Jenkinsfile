pipeline {
    agent {
        label 'Windows 10'
    }
    
    stages {
        stage('Echo') {
            steps {
                // Print a message on the console
                echo 'Hello from Windows 10 agent!'
            }
        }
    }
	
    post {
        success {
            // If the pipeline execution is successful, print a success message
            echo 'Pipeline executed successfully on Windows 10 agent!'
        }
        failure {
            // If the pipeline execution fails, print an error message
            echo 'Pipeline execution failed on Windows 10 agent!'
        }
    }
}

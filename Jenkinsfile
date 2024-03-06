pipeline {
    agent {
        label 'Windows 10'
    }
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the GitHub repository
                git branch: 'main', url: 'https://github.com/rajesh3692/Testing.git'   
            }
        }
        
        stage('Download .exe file') {
            steps {
                // Download the .exe file from the repository
                bat 'curl -O https://github.com/rajesh3692/Testing/blob/main/PING.EXE'  
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

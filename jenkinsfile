pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo "Checkout the source code from the Git repository"
                git https://github.com/tushar-dubey5/Jenkins.git'
            }
        }

        stage('Build') {
            steps {
                echo "Execute build commands or scripts"
                sh 'chmod u+x test.py'
            }
        }

        }

        stage('Deploy') {
            steps {
                echo "Deploy artifacts to a production server or environment"
                //sh 'your-deployment-command-or-script.sh'
            }
        }

        stage('Monitor') {
            steps {
                echo "Perform monitoring and verification tasks"
                //sh 'your-monitoring-command-or-script.sh'
            }
        }
    }

    post {
        success {
            // This block executes if the pipeline is successful
            echo 'Deployment was successful!'
            // Add any additional success actions here
        }
        failure {
            // This block executes if the pipeline fails
            echo ' failed!'
            // Add any failure actions or notifications here
        }
    }
}   

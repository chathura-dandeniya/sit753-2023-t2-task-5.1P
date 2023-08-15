pipeline {
    agent any

    environment {
        DIRECTORY_PATH = 'path_to_code_directory'
        TESTING_ENVIRONMENT = 'name_of_testing_environment'
        PRODUCTION_ENVIRONMENT = 'Chathura_Dandeniya'
    }

    stages {
        stage('Build') {
            steps {
                echo "Fetch the source code from the directory: ${DIRECTORY_PATH}"
                echo "Compile the code and generate any necessary artifacts"
            }
        }
        
        stage('Test') {
            steps {
                echo "Unit tests"
                echo "Integration tests"
            }
        }

        stage('Code Quality Check') {
            steps {
                echo "Check the quality of the code"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy the application to testing environment: ${TESTING_ENVIRONMENT}"
            }
        }

        stage('Approval') {
            steps {
                echo "Awaiting approval..."
                sleep(time: 10, unit: 'SECONDS')
                echo "Approved"
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying the application to production environment: ${PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}

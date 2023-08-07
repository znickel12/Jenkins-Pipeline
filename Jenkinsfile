pipeline{
    agent any
    environment {
        DIRECTORY_PATH= "/Users/rebeccanickel/.jenkins"
        TESTING_ENVIRONMENT= "SANDBOX"
        PRODUCTION_ENVIRONMENT= "Zachary Nickel"
    }
    stages{
        stage('Build'){
            steps{
                echo "fetch the source code from the directory path: $DIRECTORY_PATH"
                echo "Compile the code and generate any necessary artefacts"
            }
        }    
        stage('Test'){
            steps{
                echo "Units Tests"
                echo "Integration Tests"
            }
        }    
        stage('Code Quality Check'){
            steps{
                echo "Check the quality of the code"
            }
        }    
        stage('Deploy'){
            steps{
                echo "Deploy the application to a testing environmebnt: $TESTING_ENVIRONMENT"
            }
        }    
        stage('Approval'){
            steps{
                sleep(time: 10)
            }
        }    
        stage('Deploy to Production'){
            steps{
                echo "Deploy code to the production environment: $PRODUCTION_ENVIRONMENT"
            }
        }    
    }
}
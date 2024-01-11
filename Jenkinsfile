pipeline {
    agent any

    stages {
        stage("stage 1"){
            steps {
            echo "Build"
            echo "Job name: $JOB_NAME"
            }

        }
        stage("stage 2"){
            steps{
            echo "Test"
            }
        }
        stage("stage 3"){
            steps{
            echo "Deploy"
            }
        }
    }
}

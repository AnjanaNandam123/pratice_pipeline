pipeline {
    agent any
    environment {
        VERSION = "1.0"
    }

    stages {
        stage("stage 1"){
            steps {
            echo "Build"
            echo "BUILD VERSION NUMBER ${VERSION}"
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
          withCredentials([usernamePassword(credentialsId: 'Git Credentials', passwordVariable: 'pwd', usernameVariable: 'uname')]) {
    echo "${uname} ${pwd}"
}
            }
        }
    }
     post
    {
       
        success{
            echo "BUILD STATUS or BUILD STATUS CHANGE"

        }
       
    }
}

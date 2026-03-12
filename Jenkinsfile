pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Sahilsalunkhe001/my_first_rep.git'
            }
        }

      stage('Publish'){
        steps{
          publishHTML([
            allowMissing:true,
            alwaysLinkToLastBuild:false,
            keepAll:false,
            reportDir:'.',
            reportFiles:'test.html',
            reportName:'My HTML Pipe Publish'
           ])
        }
     }
    }
}

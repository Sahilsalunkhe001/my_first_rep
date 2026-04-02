pipeline{
  agent any
  stages{
    stage( 'Checkout'){
      steps{
            git url :'https://github.com/Sahilsalunkhe001/my_first_rep.git',branch:'master'
      }
    }
    stage('Publish'){
    steps{
      publishHTML([ 
        allowMissing:true,
        alwaysLinkToLastBuild:false,
        keepAll:false,
        reportDir:'.',
        reportFiles:'Hello.html',
        reportName:'myhtmlfile',
        ])
      }
      }
  }
}

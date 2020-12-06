pipeline {

agent any

stages {
     stage ('clone the code')
       {
          steps 
             {
                sh 'echo downloading code from github repo'
             }
        }
      
      
      stage ('build')
       {
          steps 
             {
                sh 'echo code is building'
             }
        }
      
    stage ('deploy to dev')
       {
          steps 
             {
                sh 'echo deploying pkgs on dev env'
             }
        }
      
    stage ('functional testing')
       {
          steps 
             {
                sh 'echo doing functional testing'
             }
        }
      
     stage ('Get approval from QA Manager')
     {
     input "Please approve for QA deployment?"     
     }
     
     
     stage ('deploy to QA')
       { steps { echo 'deploying pkg to QA env'}
        }
    }
    }

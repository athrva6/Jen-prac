pipeline {
   agent any
   environment {
         APP_NAME='demo-app'
            }
     stages{
        stage ('Build'){
      steps{
         echo 'Building $APP_NAME'
          }
       }
        stage ('checkout'){
       steps { checkout scm }
             }
        stage ('test'){
      steps{echo 'testing'} 
         }
   }
   post {
      success {echo 'ALL stages passed'}
      failure {echo 'something failed'}
}  
}

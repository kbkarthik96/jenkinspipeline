pipeline {
   agent { label 'master' }
   stages {
      stage ('BUILD') {
         steps {
         sh '''
         echo "this is build stage"
         sleep 5
         exit 0
         '''
         }
         }
         stage ('DEPLOY') {
         steps {
         sh '''
            sleep 5
            echo "this is deploy stage"
            '''
         }
         }
      stage ('TEST') {
         steps {
         sh '''
         sleep 5
         echo "this is test stage"
         '''
         }
      }
         }
      
}

pipeline {
   agent none
   stages {
      stage ('BUILD') {
         agent { label 'master' }
         steps {
         sh '''
         echo "this is build stage"
         sleep 5
         exit 0
         '''
         }
         }
         stage ('DEPLOY') {
            agent { label 'slave1' }
         steps {
         sh '''
            sleep 5
            echo "this is deploy stage"
            '''
         }
         }
      stage ('TEST') {
         agent { label 'slave2' }
         steps {
         sh '''
         sleep 5
         echo "this is test stage"
         '''
         }
      }
         }
      
}

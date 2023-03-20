pipeline {
   agent any
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
         parallel {
            stage ('TEST1') {
               steps {
               echo "this is test1"
               }
            }
            stage ('TEST2') {
            steps {
            echo "this is test2"
            }
               } 
            
            
           } 
         
        }
   }
}

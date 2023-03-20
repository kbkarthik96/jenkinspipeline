pipeline {
   agent any
   environment {
   name='karthik'
   }
   stages {
      stage ('BUILD') {
         steps {
         sh '''
         echo "this is build stage"
         echo "$name"
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

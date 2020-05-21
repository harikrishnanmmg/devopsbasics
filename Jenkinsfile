pipeline {
   agent any

   stages {
      stage('Hello') {
         steps {
            echo 'Hello World.. This is devops basics training'
         }
      }
      stage('shell script') {
         steps {
            sh label: '', script: '''#!/bin/sh
            date
            hostname'''
         }
      }      
   }
}

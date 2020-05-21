pipeline {
   agent any

   stages {
      stage('Hello stage') {
         steps {
            echo 'Hello World.. This is devops basics training'
         }
      }
      stage('shell stage') {
         steps {
            sh label: '', script: '''#!/bin/sh
            date
            hostname'''
         }
      }
      stage('maven stage') {
         steps {
            withMaven(jdk: 'jkd_8u252', maven: 'mvn_3.6.3') {
            sh 'mvn clean package'
            }
            archiveArtifacts 'target/helloworld-1.1.jar'
         }
      }
   }
}

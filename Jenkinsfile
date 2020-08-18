pipeline {
   agent any

   stages {
      stage('Checkout') {
         steps {
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '05e23b0e-0616-402c-85dd-4320abc54bb0', url: 'https://github.com/Lavanya-Prabhakar/Big-Billion-Sale.git']]])
         }
      }
      stage('Build') {
          steps {
              build 'build run successfully'
          }
      }
      stage('Test') {
          steps {
              echo 'Test run sucessfully'
          }
      }
      stage('QA Deploy') {
          steps {
              echo 'QA Deploy run sucessfully'
          }
      }
      stage('prod Deploy') {
          steps {
              echo 'Deployed run sucessfully'
          }
      }
   }
}

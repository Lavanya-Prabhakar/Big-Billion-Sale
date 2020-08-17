pipeline {
   agent any

   stages {
      stage('Checkout') {
         steps {
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '6b65c839-454a-4719-9ab7-453a05085ae3', url: 'https://github.com/Lavanya-Prabhakar/Big-Billion-Sale.git']]])
         }
      }
      stage('Build') {
          steps {
              build 'BBD_pipeline'
          }
      }
      stage('Test') {
          steps {
              echo 'Test sucessfully'
          }
      }
      stage('QA Deploy') {
          steps {
              echo 'QA Deploy sucessfully'
          }
      }
      stage('prod Deploy') {
          steps {
              echo 'Deployed sucessfully'
          }
      }
   }
}

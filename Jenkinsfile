pipeline {
   agent any
   
   stages {
      stage('Checkout') {
         steps {
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: '']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/joheckstrom/hello-world2.git']]])
         }
      }
      stage('Build-1') {
         steps {
            echo 'building Hello World'
        }
      }
      stage('Test-1') {
         steps {
            echo 'Testing Hello World2'
           }
      }
      stage('Hello3') {
         steps {
            echo 'Hello World3'
          }
      }
      stage('Hello4') {
         steps {
            echo 'Hello World4'  
         }
      }
   
   }
}

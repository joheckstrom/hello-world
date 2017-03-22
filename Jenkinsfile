#!groovy
node {
     stage('Checkout') {
  
            checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: '']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/joheckstrom/hello-world2.git']]])
       
      }
      stage('Build-1') {

            echo 'building Hello World'
  
      }
     stage('Test-1') {
         parallel linux: {
            node('linux1') {
               echo 'Testing Hello World2 linux'
            }
         },
         windows: {
            node('windows2') {
                  echo 'Testing Hello World2 windows'
            }
         }
      }
      stage('Deploy') {

            echo 'Hello World3'
          
      }
      stage('Check') {
       
            echo 'Hello World4'
         
      }
}

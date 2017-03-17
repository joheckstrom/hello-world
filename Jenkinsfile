node {
   stage 'Checkout'
   checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: '']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/joheckstrom/hello-world1.git']]])
   stage 'Hello1'
   echo 'Hello World'
   stage 'Hello2'
   echo 'Hello World2'
   stage 'Hello3'
   echo 'Hello World3'
   
   
}

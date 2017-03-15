node {
   stage 'Checkout'
   checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: '']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/joheckstrom/hello-world1.git']]])
   stage 'Hello'
   echo 'Hello World'
   
}

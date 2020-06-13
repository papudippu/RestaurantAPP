#!/usr/bin/env groovy
//def tomcat_home="/opt/app/home"
def docker_tag="nginx_docker_build_image:v1.0"
node ( "master"){
   stage ("checkout"){
   echo " checking out"
   checkout scm
   sh "pwd"
   }
   stage ("Build UI"){
   echo "Build UI"
   sh  "sudo docker build -t $docker_tag ."
      
   }
   stage ("Deploy Dev") {
   echo "Deploy in Dev"
   sh " sudo docker run -itd -p 9191:80 $docker_tag "
   }
} 


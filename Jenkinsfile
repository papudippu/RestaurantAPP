#!/usr/bin/env groovy
def tomcat_home="/opt/app/home"

node ( "master"){
   stage ("checkout"){
   echo " checking out"
   checkout scm
   sh "pwd"
   }
   stage ("Build UI"){
   echo "Build UI"
   sh  "sudo docker build -t 'nginx_docker_build_image:v1.0' ."
      
   }
   stage ("Deploy Dev") {
   echo "Deploy in Dev"
   }
} 


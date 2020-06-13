#!/usr/bin/env groovy
def tomcat_home="/opt/app/home"

node ( "master"){
   stage ("checkout"){
   echo " checking out"
   checkout scm
   }
   stage ("Build UI"){
   echo "Build UI"
   }
   stage ("Deploy Dev") {
   echo "Deploy in Dev"
   }
} 


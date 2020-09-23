
pipeline {
 agent any
  
 stages {
  stage("Clear Workspace") {
   steps {
    deleteDir()

   }
  }
  stage("Checkout") {
   steps {

    echo 'checkout'
    checkout scm

   }
  }
 }
}

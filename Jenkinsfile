
pipeline {
 agent {
    label 'docker' 
  }
  
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
  stage("Build") {
   steps {
    script {
     sh "docker build -t ubuntuImage . "
    }
    
   }
  }
 }
}

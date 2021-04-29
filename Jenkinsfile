pipeline {

  agent any
  
  stages{
    
    stage("KubeDeploy"){
      steps{
        sh "kubectl apply -f deploy.yaml --kubeconfig /admin.config"
      }
    }
    
  }

}

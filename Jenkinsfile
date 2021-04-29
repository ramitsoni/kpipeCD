pipeline {

  agent any
  
  stages{
    
    stage("KubeDeploy"){
      steps{
        echo "kubectl apply -f deploy.yaml --kubeconfig /admin.config"
      }
    }
    
  }

}

pipeline {

  agent any
  
  parameters {
    booleanParam(name: "isDeployPod", defaultValue: true)
  }
  
  stages{
    
    stage("KubeDeploy"){
      when{
        expression{
          param.isDeployPod
        }
      }
      
      steps{
        sh "kubectl apply -f deploy.yaml --kubeconfig /admin.conf"
      }
    }
    
  }

  post{
    success {
      echo "all good"
    }
    failure {
      echo "fails"
    }
    always {
      echo "always"
    }
    
 }  
  
}

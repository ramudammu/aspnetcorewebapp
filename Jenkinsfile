pipeline {  
 agent any  
 environment {  
  dotnet = 'C:\\Program Files\\dotnet\\dotnet.exe'  
   }  
 stages {  
  stage('Checkout') {  
   steps {
       git credentialsId: '159cc590-911a-4367-a1f6-491df39982a2', url: 'https://github.com/ramudammu/aspnetcorewebapp.git', branch: 'main'
   }  
  } 
 stage('Build') {  
   steps {  
    bat 'dotnet build %WORKSPACE%\\aspnetcorewebapp.sln --configuration Release' 
    //bat 'dotnet build C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\HRMPipelines\\jenkins-demo\\HRM\\HRM.sln --configuration Release'  
   }  
  }
 
}
 
}

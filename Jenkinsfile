pipeline{
     agent {
         label any
     }
     stages{
         stage('clone'){
             steps{
                 git url: 'https://github.com/saleor/saleor.git',
                     branch: 'main'
             }
         }
         stage('docker_image_build'){
             steps{
                 sh "docker image build -t saleor:1.0 ."
             }
         }
     }
}
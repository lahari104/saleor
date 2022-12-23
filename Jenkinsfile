pipeline{
    agent any
    stages{
        stage('clone'){
            steps{
                git url: "https://github.com/lahari104/saleor.git",
                    branch: 'main'
            }
        }
        stage('image_build'){
            steps{
                sh "docker image build -t saleor:1.0 ."
            }
        }
    }
}
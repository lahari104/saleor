pipeline{
    agent {
        label 'node-2'
    }
    stages{
        stage('clone'){
            steps{
                git url: "https://github.com/lahari104/saleor.git",
                    branch: 'main'
            }
        }
        stage('image_build'){
            steps{
                sh "docker info"
                sh "docker image build -t saleor:1.0 ."
            }
        }
    }
}
pipeline {
    agent any

    stages{
        stage('Build Stage') {
            steps{ 
                echo 'hello'
                sh 'docker build -t ferastamimi95/client-build .'

            }
        
           
        }
        stage('Checkout scm') {
            Checkout scm
        }
    }
}

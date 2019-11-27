node('master') {
    docker.withServer('unix:///var/run/docker.sock') {
        stage('Git clone') {
            git 'https://github.com/FerasTamimi201/jenkins-client-build'
        }
        }
        stage('Build') {
            docker
                sh 'docker build -t ferastamimi95/client .'
                
                sh "bash ./build.sh;"
                }
        }
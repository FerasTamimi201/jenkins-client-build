node('master') {
    docker.withServer('unix:///var/run/docker.sock') {
        stage('Git clone') {
            git 'https://github.com/FerasTamimi201/jenkins-client-build'
        }
        stage('Build') {
            docker
                .image('ferastamimi95/client-2')
                .inside('--volumes-from jenkins-master') {
                    sh "bash ./build.sh;"
                }
        }
        
        }
        
        }
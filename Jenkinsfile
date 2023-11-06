pipeline{
    agent any;
    stages{
        stage('run'){
            steps{
                sh 'pwd'
                docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("prathmeshrajmane/docker-test")

        /* Push the container to the custom Registry */
        customImage.push()
    }
            }
        }
    }
}


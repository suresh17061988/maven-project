pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                bat 'maven clean package'
                bat "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }

        }

    }
}
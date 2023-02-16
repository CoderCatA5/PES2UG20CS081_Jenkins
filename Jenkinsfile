pipeline{
    agent{
        docker{
            image 'jenkins:pes2ug20cs081'
        }
    }

    stages{
        stage('Clone Repository'){
            steps{
                git branch:'main',
                url : 'https://github.com/CoderCatA5/PES2UG20CS081_Jenkins.git'
            }    
        }
    }
}